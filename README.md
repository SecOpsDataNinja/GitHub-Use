# GitHub-Use
记录使用Git和GitHub的日常


### 建立仓库和ssh初始化
 - 首先下载git，不多做说明
 - 下载完成之后，生成密钥，由于我是windows，且不喜欢在C盘目录下，所以设置了保存密钥的路径
   ``` 
   ssh-keygen -t ed25519 -C "funokobe@gmail.com" -f D:\usage tool\dev tool\ssh 
   ``` 
- 启用ssh代理
  ~~~
  eval $(ssh-agent)
  ~~~

- 将保存的密钥添加到GitHub账户

  ~~~ 
  ssh-add "D:\usage tool\dev tool\ssh\id_ed25519" 
  ~~~
  ![ssh的位置](image-1.png)
- 测试是否可以正常连接到GitHub
  ~~~
   ssh -T git@github.com
  ~~~
  ![成功的截图](image.png)

- 配置自己的用户名和邮箱
  ~~~
  git config --global user.name "mygitcode"
  git config --global user.email "xxxxxxx@gmail.com"
  ~~~
  
- 初始化一个新的 Git 仓库
  ~~~
  gitgit init
  ~~~