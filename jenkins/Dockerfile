ARG JENKINS_VERSION=lts
FROM jenkins/jenkins:${JENKINS_VERSION}

# 将goctl 复制到 jenkins容器中
COPY ./goctl /usr/local/bin/goctl

# 修改时区
RUN cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime