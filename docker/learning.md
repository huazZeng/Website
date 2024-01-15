## Docker
### https://www.runoob.com/docker/docker-tutorial.html
### Basic Instruction
* docker run
-i 交互式操作
-t 终端
-d 后台运行
-p 设置端口

```bash
docker run -d -p 5000:5000 training/webapp python app.py
```
 * docker ps
    * -a 查看所有容器，可以重启之前容器
 * docker stop
 * docker restart
 * docker attach 进入后台容器，如果退出，则会导致后台容器退出
 * docker exec 进入后台容器（推荐），不影响后台
 * docker export 导出容器
 * docker import 导入容器快照
eg.
 ```bash
   $ cat docker/ubuntu.tar | docker import - test/ubuntu:v1
```
 * docker rm -f 删除容器
 * docker port 查看应用端口
 * docker logs -f 查看标准输出
 * docker top 查看容器内部进程
 * docker inspect 查看docker底层信息
 * docker images 查看本机镜像
    REPOSITORY:TAG  ubuntu:15.10  **15.10** 定义不同镜像
 * docker pull 获取新的镜像
 * docker search httpd 查找镜像
 * docker rmi 删除镜像
 * docker commit 在已有镜像上修改
 * docker build 创建镜像
*

###未完结
* docker makefile
* 容器内连接
* 管理工具
