# docker-lamp
Docker化lamp

## 镜像特点

- 2015/6/29 继承基础镜像docker-mysql

## 使用方法

- 获取代码并构建

        git clone https://github.com/Dockerlover/docker-lamp.git
        cd docker-lamp
        docker build -t docker-lamp .

- 运行容器

        docker run -d -it --name lamp -p 8082:80 \
        -v /var/docker_images/docker-lamp/app:/app docker-lamp
