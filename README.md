# Winter-Vacation-Record

>我现在觉得，没有什么比坚持记录自己的成长一段时间后再回头感受更有成就感的事情了。

## 2020-1-9

### 今

- 继续配[webpack](https://github.com/linbudu599/Webpack4.x-Template)，原本配好了垫片和多页面还是挺带劲的，还配了一个挺好玩的 [webpackbar](https://www.npmjs.com/package/webpackbar)，就是vuepress打包的时候会有的那两个进度条，贼有逼格。还有一个[speed-measure-webpack-plugin](https://github.com/stephencookdev/speed-measure-webpack-plugin)，在性能分析上也挺有用的，但是，但是！！全部搞完再优化了一些零碎的配置之后发现出问题了，启动后的页面里明明js和css文件都被注入了，但是js文件并不执行...，用排除法大概锁定范围在了 **optimization.splitChunks** 里，但进一步注释掉有嫌疑的配置项后发现整个模板崩了，js文件直接不被注入...，淦，我头疼。好像每天都是解决前一天遗留的 :bug:，再留给明天一只更大只的 :bug:
- 看了云谦老师关注的工具，[awesome-f2e-libs](https://github.com/linbudu599/awesome-f2e-libs)，先用的 [**projj**](https://github.com/popomore/projj) 想着管理下项目吧，结果一添加项目就报错，看了下大概一年前就有issue提这个问题了，但并没解决...，想着那算了，[**fx**](https://github.com/antonmedv/fx)看起来也不错，可以在命令行打开折叠的json对象，好的，`fx data.json` 没反应。打扰了，卑微的Windows
- [天气小应用](https://github.com/linbudu599/weather-msg-sender)用ts重构完了，但是，[那个问题](#2020-1-8)其实算不上被解决了，我最后用的方法是得到返回信息后用node写到文件里，然后别的模块再去读取、处理。因为我的思路就是要把异步返回的结果释放到全局里...
-  [ssr-github](https://github.com/linbudu599/SSR-Github)，写好首页啦，还是成就感max的，突然感觉以后用ts重构这个项目不会太简单...，明天继续写仓库详情页啥的。
- 开始学小程序咯~，但是今天就只是开了个头，稍微复习了下文档
- 家园的项目准备再推一下，把umi、dva、antd pro、react更深入一些应该会更得心应手

### 明

- 解决webpack的bug，多页面用动态入口配置？
- 继续写ssr-GitHub、小程序，瞅了一下寒假计划，感觉得再加两个线程了
- [How-to-learn-node-correctly](https://github.com/i5ting/How-to-learn-node-correctly)，写写node！
- 云谦老师B站的UMI教程
- 读一读hooks相关的文章
- 阮一峰老师的koa教程，之前一直想看来着，好像有几个知识点挺重要的
- 新线程：ts实现axios
- 新线程：graphql初体验

## 2020-1-8

### 今

- 继续配置自己的 [`webpack` 模板](https://github.com/linbudu599/Webpack4.x-Template)，主要是dll和一些零碎的地方，还剩下**垫片**和**多页面**几个地方没有处理，可能要开始准备看 `webpack5` 的alpha了？
- 用 `GitHub Actions` 配好了CD，先给自己的博客配上了，但是配上之后nginx马上崩了，不清楚有没有直接关系，观望一下。主要是感觉 `JenKins` 太折磨了，而且很多功能我远远用不上。
- 新开了个记录 `actions` 的[仓库](https://github.com/linbudu599/Enjoy-Github-Actions)，因为觉得 `GitHub Actions` 还是挺有趣强大的，玩法挺多
- 用 `typescript` 重构了之前的[天气小应用](https://github.com/linbudu599/weather-msg-sender)，同时换了API接口（淦，转化逻辑又要重写，原本的那个外国网站崩了..），但是有几个地方卡住了，又是请教大佬又是在思否提问的...
- 继续跟着视频写之前的 [`ssr-github` 项目](https://github.com/linbudu599/SSR-Github)，终于搞懂了代理接口同时区分csr/ssr的配置代码...

### 明

- 把那个天气小应用完成好，今天的主要问题是需要得到异步流程结果并且作为模块导出，看了思否大佬的回答大概有思路了
- ssr-github，开始写页面和逻辑
- **家园的项目！** 害我都忘记这一茬了...，验证码的逻辑大概解决了。可能是我写的太远了，需要的接口多了十来个...，后端同学知道估计要鲨了我
- 配完webpack剩下的部分
- 写写node和ts
