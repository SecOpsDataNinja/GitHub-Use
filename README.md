# GitHub-Use
记录使用Git和GitHub的日常


### 建立仓库和ssh初始化
 - 首先下载git，不多做说明
 - 下载完成之后，生成密钥，由于我是windows，且不喜欢在C盘目录下，所以设置了保存密钥的路径
   ``` 
   ssh-keygen -t ed25519 -C "funokobe@gmail.com" -f D:\usage tool\dev tool\ssh 
   ``` 
- 将保存的密钥添加到GitHub账户

- 将本地密钥添加到ssh
  ~~~ 
  ssh-add "D:\usage tool\dev tool\ssh\id_ed25519" 
  ~~~