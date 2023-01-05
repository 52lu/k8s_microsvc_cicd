ARG JENKINS_VERSION=lts
FROM jenkins/jenkins:${JENKINS_VERSION}

# 将goctl 复制到 jenkins容器中
COPY ./goctl /usr/local/bin/goctl
# 将kubectl文件复制到jenkins容器中
COPY ${KUBECTL_BIN_PATH} /usr/local/bin/kubectl
# 将k8s的配置.kube/config复制到jenkins容器
COPY ${K8S_KUBE_CONFIG} /root/.kube