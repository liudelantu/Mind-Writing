**规划**

全局账户 使用我自己的git账户

在公司项目的目录里，配置公司项目给我的账户

-----



**配置git账户**

```sehll
# 个人账户
git config --global user.name "liudelantu"
git config --global user.email "liudelantu@163.com"
git config --list

# 公司账户，在公司的项目目录里执行以下命令
git config user.name "Company Name"
git config user.email "company.email@example.com"
```

-----



**生成ssh密钥**

```shell
ssh-keygen -t rsa -b 4096 -C "liudelantu@163.com" -f ~/.ssh/id_rsa_liudelantu

ssh-keygen -t rsa -b 4096 -C "company.email@example.com" -f ~/.ssh/id_rsa_company

# ~/.ssh/config  这个配置文件告诉 SSH 客户端在连接到不同的 Git 服务器时使用不同的密钥
# ~/.ssh/config 内容如下:
# 配置个人 GitHub 账户
Host github-liudelantu  # github-liudelantu 用来区分不同账户
  HostName github.com
  User git
  IdentityFile ~/.ssh/id_rsa_liudelantu
# 配置公司 GitHub 账户
Host github-company
  HostName github.com
  User git
  IdentityFile ~/.ssh/id_rsa_company
  

然后把生成的公钥 .pub 结尾的内容，复制到github的ssh key里

克隆个人项目：
git clone git@github-liudelantu:liudelantu/Mind-Writing.git

克隆公司项目：
git clone git@github-company:companyname/repository.git

```

-----



**git操作**

```shell
git status
git add <file>
git commit -m "commit message"
git log

git branch <branch-name>
git checkout <branch-name>
git merge <branch-name>
git push origin <branch-name>
git pull
git branch -d <branch-name>
git remote -v

```

