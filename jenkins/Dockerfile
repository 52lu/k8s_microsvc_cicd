ARG JENKINS_VERSION=lts
FROM jenkins/jenkins:${JENKINS_VERSION}

# 将goctl 复制到 jenkins容器中
COPY ./goctl /usr/local/bin/goctl

# 修改时区
#定义时区参数
ENV TZ=Asia/Shanghai

