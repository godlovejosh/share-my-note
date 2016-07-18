## 安装Git
#### Windows和Mac可以使用GUI安装方式,下载地址:<https://git-scm.com/>
#### Mac和Linux也可以选择源码包安装方式,下载地址:<https://www.kernel.org/pub/software/scm/git/>

### 安装完成后简单的配置一下:
1. git config --global user.name “Your Name”
2. git config --global user.email “you@example.com”
3. git config --global push.default matching

克隆远程版本库：
git clone git@github.com:godlovejosh/share-my-note.git

克隆本地版本库：
git clone /path/to/my/workspace/demo /path/to/my/workspace/demo-backup

* 用法1：git clone \<repository> \<directory>
* 用法2：git clone --bare \<repository> \<directory>
* 用法3：git clone --mirror \<repository> \<directory>

## 常见的gitignore
    echo “
    bin
    .metadata
    */bin
    */.project
    */.classpath
    */target
    */.settings
    */logs
    target
    */target
    .settings
    .project
    .DS_Store
    .idea/
    *.iml
    .classpath
    */src/test/java/META-INF/MANIFEST.MF
    zookeeper.out” >> .gitignore

* cat .git/refs/heads/master 查看master分支指向的提交ID是否改变了
* git log --graph --oneline 提交之后查看
* git reset --hard HEAD^ 重置到上一个老的提交（父提交）
* git reset --hard 938a761 重置到任意一次提交
* 用法一：git reset [-q] [\<commit>] [--] \<paths>...
* 用法二：git reset [--soft | --mixed | --hard | --merge | --keep] [-q] [\<commit>]
1. 替换引用的指向。引用指向新的提交ID；
2. 替换暂存区。替换后，暂存区的内容和引用指向的目录树一致；
3. 替换工作区。替换后，工作区的内容变得和暂存区一致，也和HEAD所指向的目录树内容相同。


* 重置暂存区(commit之前的操作)：与git add . 相反的操作是 git reset HEAD，与git add filename 相反的操作是git reset -- filename或者是git reset filename;（默认省略--mixed参数，引用指向和暂存区都替换掉）
### 重置提交（commit之后的操作）：
* git reset --soft HEAD^
* git reset HEAD^ 或者 git reset --mixed HEAD^
* git reset --hard HEAD^(彻底撤销)

### 重置push（push之后的操作，反转提交）：
* git show HEAD
* git revert HEAD (编辑器中修改完提交说明之后，保存退出即可)
* git log --stat -2

* git --help
* git help -a

* git --exec-path 查看所有的git子命令:
* git status 显示工作区文件状态
* git add 添加到暂存区
* git reset 重置暂存区
* git branch 分支管理
* git checkout 检出到工作区、切换或创建分支
* git clean 清除工作区未跟踪文件
* git clone 克隆版本库
* git commit 提交
* git config 查询和修改配置
* git describe 通过里程碑直观地显示提交ID
* git diff 差异比较
* git difftool 调用图形化差异比较工具
* git fetch 获取远程版本库的提交
* git grep 文件内容搜索定位工具
* git gui 基于Tcl、Tk的图形化工具，侧重提交等操作
* git init 版本库初始化
* git log 显示提交日志
* git merge 分支合并
* git mergetool 图形化冲突解决
* git pull 拉回远程版本库的提交
* git push 推送至远程版本库
* git remote 远程版本库管理
* git reset 充值改变分支“游标”指向
* git rm 删除文件
* git show 显示各种类型的对象
* git stage 同义词，等同于git add
* git stash 保存和恢复进度
* git tag 里程碑管理
* git show-branch 显示分支列表及拓扑关系
* git show-ref 显示本地引用

gitk 图形管理工具：

本地commit了多个版本，一直没有push；
git冲突


修改完 用sourcetree 标记解决冲突；

get:org.apache.ibatis.binding.BindingException: Invalid bound statement (not found): com.wbm.carriage.tp.shop.dao.ShopDAO.selectOneByUid
表示找不到 DAO，先看方法在不在DAO中，然后找xml，最后看 单元测试的mybatis-config.xml有没有配置service；
kangchenjunga中 引入 xixia 的 itemService和itemDAO是没有办法的，会提示 找不到资源，去pom中查看，因为 kangchenjunga项目没有依赖xixia，跨项目了；单元测试 是 做不了了；
需要启动gateway，gateway把他们依赖起来，远程调用；








