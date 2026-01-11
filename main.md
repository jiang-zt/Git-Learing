# My Git Learning NoteBook


### git int 在当前文件夹创建工作区
### git clone http://... 克隆远程仓库到当前工作区

## 关联到远程仓库
 - 只创建链接不复制代码
#### 添加远程仓库（使用 SSH 地址）
git remote add origin git@github.com:你的用户名/仓库名.git
#### 添加远程仓库（使用 HTTPS 地址）
git remote add origin https://github.com/你的用户名/仓库名.git

## 工作区--缓存--远程仓库
### git diff 查看本地工作区与暂存区的差异
### git diff --cached 比较暂存区与最新提交的差异
### git status 查看当前工作区状态

### git add <文件名> 提交文件到暂存区
### git add .   提交所有修改文件到暂存区

### git commit -m  "infos about commit" 提交暂存区文件到本地仓库
### git commit -a -m  "infos about commit" 一步到位--自动将所有已跟踪文件修改加入暂存区

## 分支
### git branch 查看所有本地分支,当前分支有*标记
### git checkout -b <分支名> 创建并切换到新分支
### git checkout <分支名> 切换到指定分支
### git merge <分支名> 合并指定分支到当前分支
### git diff <分支名> 比较当前分支与指定分支的差异
### git branch -d <分支名> 删除指定分支

## 合并
### git checkout main 
### git merge feature 

### 情况1:main 分支有更新（自动非快进）
- ```
- ```          A---B---C feature
- ```         /
-   D---E---F---G main
### 创建合并提交 H

### 情况2:main 分支无更新 main 直接指向 C
- ``` D---E---F---A---B---C

### git merge --no-ff 强制创建合并提交-非快进


### git fetch 获取远程状态
### git pull 合并
### git push 推送

### git stash 暂存工作区
### git stash pop 恢复最近一次暂存
