# GIT常见问题
*Author: Wang Xiaoqiang<wang_xiaoq@126.com> 2014.09.09*

## 撤销上次的push
两条命令：

*  `git reset --hard HEAD^`
*  `git push origin master --force`

## 撤销上次commit
* `git reset --hard NUMBER`  
其中NUMBER为要恢复到的版本，也就是执行`git log`时，后面出现的一长串ID。

## 查看某个文件的更新过程
* `git log -p filename`

## 查询当前的用户和邮箱
* `git config --list`

## 创建共享仓库（组成员共享仓库）
在初始化仓库时，使用命令：

* `git init --bare --share`
