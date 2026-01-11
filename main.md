# My Git Learning NoteBook


### git int 在当前文件夹创建工作区
### git clone http://... 克隆远程仓库到当前工作区

## 关联到远程仓库
 - 只创建链接不复制代码
#### 添加远程仓库（使用 SSH 地址）
git remote add origin git@github.com:你的用户名/仓库名.git
#### 添加远程仓库（使用 HTTPS 地址）
git remote add origin https://github.com/你的用户名/仓库名.git

### git diff 查看本地工作区与暂存区的差异
### git diff --cached 比较暂存区与最新提交的差异
### git status 查看当前工作区状态

### git add <文件名> 提交文件到暂存区
### git add .   提交所有修改文件到暂存区

### git commit -m  "infos about commit" 提交暂存区文件到本地仓库
### git commit -a -m  "infos about commit" 一步到位--自动将所有已跟踪文件修改加入暂存区
