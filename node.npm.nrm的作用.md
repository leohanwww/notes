Node.js 是一个开源与跨平台的 JavaScript 运行时环境。







NPM是随同NodeJS一起安装的包管理工具，能解决NodeJS代码部署上的很多问题，常见的使用场景有以下几种：

- 允许用户从NPM服务器下载别人编写的第三方包到本地使用。
- 允许用户从NPM服务器下载并安装别人编写的命令行程序到本地使用。
- 允许用户将自己编写的包或命令行程序上传到NPM服务器供别人使用。





1.nrm

nrm(npm registry manager )是npm的镜像源管理工具，有时候国外资源太慢，使用这个就可以快速地在 npm 源间切换

2.安装nrm

在命令行执行命令，npm install -g nrm，全局安装nrm。

3.使用

执行命令nrm ls查看可选的源。

> nrm ls                                                                  
>
> *npm ---- https://registry.npmjs.org/
>
> cnpm --- http://r.cnpmjs.org/
>
> taobao - http://registry.npm.taobao.org/
>
> eu ----- http://registry.npmjs.eu/
>
> au ----- http://registry.npmjs.org.au/
>
> sl ----- http://npm.strongloop.com/
>
> nj ----- https://registry.nodejitsu.com/

其中，带*的是当前使用的源，上面的输出表明当前源是官方源。

5.切换

如果要切换到taobao源，执行命令nrm use taobao。

6.增加

你可以增加定制的源，特别适用于添加企业内部的私有源，执行命令 nrm add <registry> <url>，其中reigstry为源名，url为源的路径。

> nrm add registry http://registry.npm.frp.trmap.cn/

7.删除

执行命令nrm del <registry>删除对应的源。

8.测试速度

你还可以通过 nrm test 测试相应源的响应时间。

> nrm test npm 

