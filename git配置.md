# git配置

配置github用户名和邮箱

```
git config --global user.name woodensRangerWZJ
git config --global user.email 13029768866@163.com
```

查看配置项

```
git config --list
```

配置秘钥

```
ssh-keygen -t rsa -C "13029768866@163.com"
输入两次密码
```

查看公钥

```
cat ~/.ssh/id_rsa.pub
```

github配置

```
登陆你的github帐户。点击你的头像，然后 Settings -> 左栏点击 SSH and GPG keys -> 点击 New SSH key
```

验证是否成功

```
$ ssh -T git@github.com
```

解决每次需要输入密码问题

```
git config --global credential.helper store
```

