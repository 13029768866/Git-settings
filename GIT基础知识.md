# Linux简单指令

1. ls  -l/-a:	 查看当前目录结构（-a:查看所有的，包含隐藏的）
2. cd xxx:      进入到特定文件
3. mkdir:       创建文件夹
4. touch:       创建空文件
5. vi:               i=>进入插入模式      ESC + WQ 保存并且退出
6. echo          向指定文件输入内容
7. cat              查看文件中的内容
8. cp               拷贝
9. rm              删除    -r（递归删除）   -f（强制删除）

# GIT的常规流程

## 1、分区

1. 工作区：写代码
2. 暂存区：临时存放每一次修改代码，没有生成历史版本
3. 历史区：存放所有历史版本

## 2、流程

1. 初始化 git init
2. 工作区  --> 暂存区     git add .
3. 暂存区  -->  历史区    git commit -m"备注"

## 3、指令

1、git rm --cached  xxx   把暂存区某个文件撤回到工作区   

​	（-r）撤销暂存区中所有提交的   

​	（-f）强制删除暂存区的某一个文件

2、git checkout xxx   把暂存区上次提交的内容撤回到工作区（覆盖工作区新写的内容）

3、git  diff  工作区VS暂存区   

​	  master（工作区vs历史区master分支）  

​	  --cached(暂存区vs历史区)

4、git  log    查看历史版本

​      git relog   查看所有历史版本

## 4、代码回滚

1、git checkout .	暂存区上次提交的内容撤回到工作区（覆盖工作区新写的内容）

2、git reset --hard 版本号  历史区中回退的某一个版本（强制改变工作区和缓存区）

## 5、分支查看

1、git branch           			查看当前存在分支

2、git branch xx 		 		创建分支

3、git checkout -b xxx		创建并切换分支

4、git satsh						  暂存文件

5、git merge xxx				 合并分支

