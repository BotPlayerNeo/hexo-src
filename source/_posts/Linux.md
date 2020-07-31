---
title: Linux
date: 2020-07-31 21:29:21
tags:
---

# SSH config文件

路径:

- 用户配置:~/.ssh/config
- 系统配置:/ssh/ssh_config

打开配置文件

```
vim ~/.ssh/config
```

常用配置文件内容

```
Host myhost                 # 别名
HostName myhost.com         # 主机名
Port 22                     # 端口默认22
User root                   # 用户名
IdentityFile ~/.ssh/id_rsa  # 密钥文件的路径
IdentitiesOnly yes          # 只接受SSH key 登录
```

使用:

```
ssh myhost
```
