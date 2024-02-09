# 使用一个基础的Web服务器映像作为父镜像
FROM nginx:latest

# 设置工作目录为 /usr/share/nginx/html
WORKDIR /usr/share/nginx/html

# 将当前目录下的所有文件复制到容器的 /usr/share/nginx/html 目录下
COPY . .

# 设置环境变量 WS_BACK_URL，指定后端服务的URL
ENV WS_BACK_URL=http://backend-service:5000

# 暴露容器的80端口
EXPOSE 80

# 设置容器的入口点为nginx启动命令
ENTRYPOINT ["nginx", "-g", "daemon off;"]

