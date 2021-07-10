# k8s
k8s

本dockerfile是一个简单的打包可运行程序的事例。

比如，把编译完成的二进制可执行文件命名为【webserver】，放在Dockerfile的同目录下。

然后运行以下命令来构建镜像：
docker build -t webserver:1.0 .

运行以下命令用刚构建的镜像来启动容器：
docker run -d -p 80:80 --name myweb webserver:1.0

验证：
可以在主机（或公网）请求本机IP：80
