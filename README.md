# k8s_microsvc_cicd

## 1.使用步骤
```shell
# 第一步: 创建持久卷，并赋权
$ mkdir volumes && chmod 777 volumes

# 第二步: 复制环境变量
$ cp env-exampl .env

# 第三步: 修改.env
# - 把GITEA_HOST修改你服务器对应的IP
 

```

## 2.启动Jenkins
```shell
# 1.启动服务(需要等一会儿)
$ docker-compose up -d jenkins
# 2.进入容器
$ docker-compose exec  jenkins bash
# 3.查看密码
$ cat /var/jenkins_home/secrets/initialAdminPassword
086d0f60b9e74ed1a8dead9e0958b471
# 4.访问服务 http://127.0.0.1:19090/
# 5.根据引导进行安装
```