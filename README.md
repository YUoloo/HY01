这是一个源于尚硅谷基于类的ioc组件管理，是自己的一个学习内容，也是我第一次使用git bash，实现将本地仓库，暂存仓库，远程仓库，联系起来的第一次尝试，根据xhs上面的步骤，成功完成了这一次操作，开心开心，再来回顾一下自己的操作
1.首先要在需要的项目中打开git 
2.运用命令 git init 进行初始化
3.把文件加载到本地仓库中 先用 git add . 加载到暂存区 
4.再使用 git commit -m "提交备注" 把文件从暂存区提交到本地仓库
5.git log 可以查看提交的记录，其中如果代码崩掉想回到以前版本运用的指令是 git reset -hardcommitID
6.（其中会有黄色文字提醒即ID，想回到哪个版本就用哪个ID）
git branch 分支名 --> 这个命令是创建分支 git branch -->查看分支, git checkout 分支名 -->跳转分支， git checkout -b 分支名 -->新建分支并跳转到该分支
git merge 分支名 -->把新分支合并到当前分支，git -graph -pretty=oneline -all -->这个也是查看分支
7.发表到远程仓库 git remote add orign url/ssh url/ssh需要在自己仓库去看
8.然后git push -u orign master orign是需要仓库的别名，master是远程仓库分支名，后续直接使用git push 就可以了
如果要使用别人的代码 就可以使用 git clone url
git fetch orign master 把更新的东西抓取到本地，但不是合并
git pull orign master 抓取并且合并
