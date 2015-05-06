#什么是Grunt？
Grunt是一个JS自动化构建工具，对于需要反复重复的任务，例如压缩（minification）、编译、单元测试、linting等，自动化工具可以减轻你的劳动，简化你的工作。

Grunt官网：
http://gruntjs.com

Grunt中文网：
http://gruntjs.net

#如何安装Grunt？
Grunt安装需要先安装node NPM。

    $ npm install grunt

可参考个人博客：
http://dandananddada.github.io/frontend/grunt

#如何使用本项目？
1.首先确保本机装有node npm。

2.clone项目到本地。

    $ git clone https://github.com/dandananddada/helloGrunt.git

3.进入项目根目录，安装所需插件。

    $ npm install

4.在app目录下创建你自己的静态资源文件。

执行grunt命令会在dist目录下生成相应处理后的资源文件。

#本项目定制的命令
查看全部命令

    $ grunt -h

清理dist目录

    $ grunt clean

将sass文件编译为css文件

    $ grunt compile

分别合并js和css文件为一个文件

    $ grunt combine

保持原目录结构混淆压缩css文件和js文件

    $ grunt compress

部署js文件和css文件（分别将js和css文件合并混淆压缩为一个文件）

    $ grunt build

启动js单元测试服务

    $ grunt test
将当前站点作为服务启动

    $ grunt server