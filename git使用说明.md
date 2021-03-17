#git 指南
## git地址
git remote origin set-url [githubrul]
也可以
git remote rm origin
git remote add origin [url]
或者仓库问价夹里面的config文件

这样可以指定origin地址
## 关于连不上的问题
设置代理
git config --global https.proxy https://127.0.0.1:2802
git config --global http.proxy http://127.0.0.1:2802
这里后面的端口查看代理设置那里

如果是sock5
socks5://127.0.0.1:2801

之后一般没openssl问题

主要ssl文件要在电脑生成,在github 更新

##使用，或者上传

这里的话，就使用
git pull 先进行下载
特定分支
git pull origin [分支名]
git pull origin feature-zhangduhuang --allow-unrelated-histories --这一句是无视历史冲突


之后在idea显示 远程分支

在setter设置里面可以填写github账号

冲突时，可以先选中右上角的下箭头，进行冲突处理
上箭头进行提交

提交之后才能push

这里还需要进行本地和远程仓库的映射
git branch --set-upstream-to=origin/feature-zhangduhuang feature-zhangduhuang
例如

进行push时（git命令在你的仓库文件夹下）
git push origin githubname:[分支名]

