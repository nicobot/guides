Ember 的起步是很容易的。Ember 使用命令行构建工具 Ember CLI 来创建和管理项目。 该构建工具有如下特性：

* 现代化静态资源管理(包括文件合并、压缩，以及版本控制)。
* 帮助创建组件、路由及更多的生成器。
* 常规的项目结构使得既有的 Ember 应用程序也很容易套用。
* 通过 [Babel](http://babeljs.io/docs/learn-es2015/) 项目支持 ES2015／ES6 JavaScript。 这也包含了对于 [Javascript 模块](http://exploringjs.com/es6/ch_modules.html)的支持，本指南将通篇使用这一特性。
* 完整的 [QUnit](https://qunitjs.com/) 测试集成。
* 强健的[Ember Addons](https://emberobserver.com/)插件生态.

## 依赖

### Git

Ember 需要 Git 来管理许多它依赖的东西。 Mac OS X 和大多数 Linux 发行版都自带有 Git. Windows 用户可以下载并运行 [this Git installer](http://git-scm.com/download/win)来安装Git.

### Node.js 和 npm

Ember CLI is built with JavaScript, and requires the most recent LTS version of the [Node.js](https://nodejs.org/) runtime. 它还需要通过 [npm](https://www.npmjs.com/) 来获取依赖的模块和软件包。 npm 是打包在 Node.js 中的，所以如果你的电脑只需要安装 Node.js 就可以了。

If you're not sure whether you have Node.js or the right version, run this on your command line:

```bash
node --version
npm --version
```

如果看到 *"command not found"* 错误或是过期版本的 Node：

* Windows or Mac users can download and run [this Node.js installer](http://nodejs.org/en/download/).
* Mac 用户通常喜欢使用 [Homebrew](http://brew.sh/) 安装 Node。安装好 Homebrew 后，运行 `brew install node` 来安装 Node.js。
* Linux用户可参考[使用Nodejs安装手册](https://nodejs.org/en/download/package-manager/).

如果你看到 npm 是过期版本，运行命令 `npm install -g npm`重新安装.

### Bower

Ember需要使用Bower管理更多的依赖包。Bower是一个使用npm安装的命令行工具。安装命令如下： ```npm install -g ember-cli```

### Watchman(可选)

在 Mac 和 Linux 上，你可以通过安装 [Watchman](https://facebook.github.io/watchman/docs/install.html) 来提高文件变化监测的性能。.

### PhantomJS(可选)

PhantomJS 可以帮助你在命令行运行测试而不需要打开浏览器。详细请查看 [PhantomJS 下载指南](http://phantomjs.org/download.html)。.

## 安装

使用 npm 安装 Ember：

```bash
npm install -g ember-cli
```

若要验证是否安装成功，请运行下面的命令：

```bash
ember -v
```

如果显示出了版本号，说明你安装成功了。