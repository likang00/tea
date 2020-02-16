# https://likang.ink/tea

## 关于Hexo: 一款基于Node.js的静态博客框架

```
git config user.name
git config user.email
```

## 准备工作
1.安装 node
2.安装 hexo-cli
`npm install hexo-cli -g`
3.cmd
`hexo init xxx`
`cd xxx`


## Hexo命令
```
hexo new "postName" #新建文章
hexo new page "pageName" #新建页面
hexo generate #生成静态页面至public目录
hexo server #开启预览访问端口（默认端口4000，'ctrl + c'关闭server）
hexo deploy #部署到GitHub
hexo help  # 查看帮助
hexo version  #查看Hexo的版本
```


## git
```
echo "# tea" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/Likang00/tea.git
git push -u origin master
```


```
博客添加图片方法：

First
1 把主页配置文件_config.yml 里的post_asset_folder:这个选项设置为true
2 在你的hexo目录下执行这样一句话npm install hexo-asset-image --save，这是下载安装一个可以上传本地图片的插件，来自dalao：dalao的git
3 等待一小段时间后，再运行hexo n "xxxx"来生成md博文时，/source/_posts文件夹内除了xxxx.md文件还有一个同名的文件夹
Second
4 最后在xxxx.md中想引入图片时，先把图片复制到xxxx这个文件夹中，然后只需要在xxxx.md中按照markdown的格式引入图片：
![你想输入的替代文字](xxxx/图片名.jpg)
注意： xxxx是这个md文件的名字，也是同名文件夹的名字。只需要有文件夹名字即可，不需要有什么绝对路径。你想引入的图片就只需要放入xxxx这个文件夹内就好了，很像引用相对路径。
5 最后检查一下，hexo g生成页面后，进入public\2017\02\26\index.html文件中查看相关字段，可以发现，html标签内的语句是<img src="2017/02/26/xxxx/图片名.jpg">，而不是<img src="xxxx/图片名.jpg>。这很重要，关乎你的网页是否可以真正加载你想插入的图片。

```


<!-- https://www.jianshu.com/p/b9f96b992b68 -->
