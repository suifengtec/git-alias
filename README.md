# Git

[Pro Git](https://git-scm.com/book/en/v2)

## Git Config

### 进行配置
```

git config --global core.autocrlf false

git config --global alias.co checkout
git config --global alias.cor "checkout -b"
git config --global alias.br branch
git config --global alias.cii "commit -m 'init'"
git config --global alias.cim "commit -m"

git config --global alias.pm "push -u origin master"

git config --global alias.cg "config --global"
git config --global alias.cgu "config --global --unset"
git config --global alias.cgl "config -l --global"

git config --global alias.lol "log --oneline"
git config --global alias.lolg "log --oneline --graph"
git config --global alias.lolga "log --oneline --decorate --graph --all"

git config --global alias.mw "merge --no-ff -m"

```


别名的使用:
```

git co [要检出的分支]
git cob [要新建并切换到的分支]

git mw "合并的备注" [要合并过来的分支]

git cii : 提交并添加初始化的备注;
git cim "提交备注";

git pm : 提交到远程的 master 分支;

git cg : 后可跟相关的指令;

git cgl: 列出 global 配置;

git cgu [要删除的配置]: 删除特定的配置;




```


### 删除一个配置
```

git config --global --unset alias.ci

```

### 查看配置
```
git config --list --system
git config --list --global
git config --list --local
git config -l
```
