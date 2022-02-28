# dockerfiles
dockerfiles

# 重新构建
# http_proxy - 代理服务器
# docker build --no-cache --build-arg http_proxy="http://172.26.208.1:7890" --build-arg https_proxy="http://172.26.208.1:7890" -t workspace -f workspace/ubuntu .

# 启动新创建的镜像
# docker run -itd -v /e/Codes:/data --privileged=true -p 2222:22 --name workspace workspace

# copy ssh keyfiles to .ssh目录
# 

# 保存镜像
# docker commit -m "copy ssh" <CONTAINER ID> workspace:v1