---
typora-copy-images-to: media
---

# Github的使用

## Connecting to GitHub with SSH

https://help.github.com/articles/testing-your-ssh-connection/

## 设置账号和EMail

- 本地设置

```
$ git config user.name "John Doe"
$ git config user.email johndoe@example.com
```

本地设置的账号和密码存储在 .git/config中

- 全局设置

```
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```

全局设置的账号和密码存储在系统目录中

## 新建一个仓储

- 服务端新建一个仓储

  ![1510909196118](media/1510909196118.png)

- 本地初始化git

  - 一般git目录会有三个文件

    ![1510909215181](media/1510909215181.png)

  - 初始化的命令

    ```
    // 初始化.git文件夹
    git init
    // 文件添加到暂存区
    git add .
    // 提交到本地仓储
    git commit -m 'init'
    // 设置origin
    git remote add origin 'git@github.com:goddlts/usegithub.git'
    // 提交到服务器的仓储的master分支
    git push origin master
    ```

    ​
