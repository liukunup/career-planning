# 面试八股文

各编程语言面试八股文收录与实战

1. 帮助阅读者重构知识体系
2. 助力求职者复习基础知识

## 收录清单

注意：当同时部署多个Notebook时，请使用不同端口号～

- [C&C++](八股文之C&C++.ipynb)

  安装部署

  ```shell
  # 镜像拉取
  docker pull datainpoint/xeus-cling-notebook:latest
  # 镜像部署（默认密码为123456）
  docker run -d \
    -p 8888:8888 \
    -e JUPYTER_ENABLE_LAB=yes \
    -e GRANT_SUDO=yes \
    --restart=always \
    --name=xeus-cling-notebook \
    datainpoint/xeus-cling-notebook:latest start-notebook.sh \
    --NotebookApp.password='argon2:$argon2id$v=19$m=10240,t=10,p=8$LaE/ahJVX6KHFhkYvwPv9w$BN+q+SBvJlcFn41qEIUq2GMT/TapRZcoiPeJfmvyqdA'
  ```

  登陆体验 [Notebook for C&C++](http://localhost:8888/)

- Java

- [Python](八股文之Python.ipynb)

  安装部署

  ```shell
  # 镜像拉取
  docker pull jupyter/minimal-notebook:latest
  # 镜像部署（默认密码为123456）
  docker run -d \
    -p 8888:8888 \
    -e JUPYTER_ENABLE_LAB=yes \
    -e GRANT_SUDO=yes \
    --restart=always \
    --name=minimal-notebook \
    jupyter/minimal-notebook:latest start-notebook.sh \
    --NotebookApp.password='argon2:$argon2id$v=19$m=10240,t=10,p=8$LaE/ahJVX6KHFhkYvwPv9w$BN+q+SBvJlcFn41qEIUq2GMT/TapRZcoiPeJfmvyqdA'
  ```

  登陆体验 [Notebook for Python](http://localhost:8888/)
