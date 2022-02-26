# dockerfiles
dockerfiles

# 重新构建
# http_proxy - 代理服务器
# docker build --no-cache --build-arg http_proxy="http://172.26.208.1:7890" --build-arg https_proxy="http://172.26.208.1:7890" -t workspace -f workspace/ubuntu .

# 启动新创建的镜像
# docker run -itd -v workspace:/data --privileged=true -p 2222:22 --name workspace workspace /sbin/init

# 启动sshd
# docker exec -it <CONTAINER ID> zsh
# sudo service ssh start

# 保存镜像
# docker commit -m "start sshd service" <CONTAINER ID> workspace:v1