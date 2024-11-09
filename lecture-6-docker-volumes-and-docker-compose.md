# 📘 Lecture 6: Docker Volumes and Docker Compose

#### 📌 Topics of Lecture

1. **Docker Volume**: Types of Volumes and Bind Mounts
2. **Docker Compose**: Multi-Container Applications and YAML Configuration

***

#### 📂 Docker Volume

* **Docker Volumes**: Persist data and allow sharing between containers.
  * Volumes are stored in Docker-managed directories (e.g., `/var/lib/docker/volumes/` on Linux).
  * Volumes can be created explicitly or during container creation.

**Types of Volumes**

1. **Anonymous Volumes**:
   * Not assigned a specific name; Docker assigns a unique identifier.
   *   Example:

       ```bash
       bashCopy codedocker run -d --name httpd_c -v /containervol httpd
       ```
2. **Named Volumes**:
   * Explicitly named and mounted for easier management.
   *   Example:

       ```bash
       bashCopy codedocker run -d --name httpd_c -v hostvol:/containervol httpd
       ```

**🔗 Bind Mounts**

* Allows mounting a host file or directory into a container using an absolute or relative path.
* Can be modified by both Docker and non-Docker processes.
*   Example:

    ```bash
    bashCopy codedocker run -d --name httpd_c -v /home/ubuntu/hostvol:/containervol httpd
    ```

**💡 Exam Questions**:

1. Differentiate between anonymous and named Docker volumes.
2. Explain the concept of bind mounts and provide an example command.

***

#### 📦 Docker Compose

**Docker Compose** allows defining and running multi-container applications using a YAML file to simplify environment setup.

**Docker Compose Commands**

1.  **Up**: Starts services in the background.

    ```bash
    bashCopy codedocker-compose up -d
    ```
2.  **Down**: Stops and removes containers, networks, and volumes.

    ```bash
    bashCopy codedocker-compose down
    ```

**📝 YAML Configuration**

* **YAML (YAML Ain’t Markup Language)** is used for Compose configuration files.
  * **File Extension**: `.yaml` or `.yml`
  * **Indentation**: Uses spaces for structure, and comments begin with `#`.

**Docker Compose Example: WordPress**

```yaml
yamlCopy codeversion: '3.1'
services:
  wordpress:
    image: wordpress
    ports:
      - 8080:80
    environment:
      WORDPRESS_DB_HOST: db
      WORDPRESS_DB_USER: exampleuser
      WORDPRESS_DB_PASSWORD: examplepass
      WORDPRESS_DB_NAME: exampledb
    volumes:
      - wordpress:/var/www/html
  db:
    image: mysql:8.0
    environment:
      MYSQL_DATABASE: exampledb
      MYSQL_USER: exampleuser
      MYSQL_PASSWORD: examplepass
      MYSQL_RANDOM_ROOT_PASSWORD: '1'
    volumes:
      - db:/var/lib/mysql
volumes:
  wordpress:
  db:
```

**Steps**:

1. Create a directory (e.g., `my_wordpress`), navigate into it, and create a `docker-compose.yml` file with the above content.
2.  Run the environment using:

    ```bash
    bashCopy codedocker-compose up -d
    ```

**💡 Exam Questions**:

1. Describe the purpose of Docker Compose and how it is used with YAML.
2. Write a basic Docker Compose YAML file to set up a WordPress and MySQL environment.
