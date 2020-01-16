# Winter-Vacation-Record

>我现在觉得，没有什么比坚持记录自己的成长一段时间后再回头感受更有成就感的事情了。

## **遗留&进行中**

- hooks :construction:
- graphql :sparkles:
- Umi & Dva ​&​ ​A​n​td​ ​P​ro​ ​&​ ​家园项目:whale:
- useAxios :fire:
- 逃避闭包&useRef，why and why not。:ambulance:

## 2020-1-16

### 今

- useAxios，作者回复了issue，但是我今天再看发现估计是我自己的问题，可能又是闭包的锅，准备明天沉下心来再推翻重来。
- ssr-github，issues界面比我想得难不少...，进度得再推后一到两天，哈哈哈哈想把部署环节当成奖励。今天发现了几个可以再度优化的点：
  - 是否需要把封装过的 `api请求方法` 再封装一层，或者提高原来的封装程度，但这样会不会过于耦合了？
  - 有几个组件感觉还能复用，尤其是拆分成多个文件，但这样可能会影响 `getInitialProps` 或者使得数据流更复杂？需要思考下组件复用的相关思维了
- ts-axios，继续完成了拦截器部分，越来越庞大了整个结构，但是也越来越兴奋了，ts真的太适合用来写这种复杂应用了。
- dracula，一个新的仓库，主要是之前看了英剧德古拉之后觉得伯爵吸了别人的血就拥有了别人的记忆、能力这点很有意思哈哈哈哈哈。主要突然有这个想法也是因为在群里看到一个学弟自己写的一个npm包 [inob](https://github.com/kidonng/inob)，自叹弗如。再次遗憾自己要是大一就进家园就好了。不求像一些神仙一样小学开始学VB啥的。

#### 明

- puppeteer，搞一下基本操作，把之前看的那本ts入门教程爬下来试试
- feflow的使用！一直想学一下来的
- 完善ssr-github到可部署上线阶段
- ts-axios，跟进到测试部分之前
- h5（孙哥哥的那个仓库）

## 2020-1-15

### 今

- ts-axios 基础工作已经完成，准备开始后续的拦截器、cancelToken部分，我说axios源码怎么有15k呢...，这考虑的是真的多。学习到了typescript继承内置对象Error时需要手动 `Object.setPrototypeOf(this, AxiosError.prototype)` 一下。然后就是觉得这个思路如果让我自己来写起码要有一年工作经验才能写得出来，各处泛型、将类实例和函数结合到一起的思路等等。
- ssr-github已经接近尾声，剩余issues界面的开发，感觉很喜欢这个老师的授课方式，和你一起把坑踩一遍，然后告诉你为啥这是个坑，或者推翻重来告诉你如何提高程序性能（缓存、复用等）。应该会继续完善下去，毕竟GitHub API那么完善。如果next支持ts的话也准备用ts重构一下，感觉这个项目还是挺有必要的，各种各样的数据类型、函数重载等。
- 准备开始搞puppeteer的时候，被安排的明明白白，因为担心只下core可能以后搞大的不够，所以下的完整版，但是一下下了半个小时，所以我就只能孤零零的整个README放上学习资源。

### 明

- puppeteer的基础使用，完成部分功能如爬虫、合并PDF，考虑基于puppeteer写个爬虫工具，React+TS+Koa+MongoDB？再议
- ssr-github，完成、样式调整、撰写文档、测试（暂无）、部署上线，github.linbudu.top
- ts-axios，继续推进
- 准备开始移动端的学习了

## 2020-1-14

### 今

- ssr-github与ts-axios进展顺利，准备给ts-axios写下具体的分析文档，作者的思路有点跳跃，需要缓缓。
- useAxios卡住了，估计不是我的理解问题，去作者源码看了一下，作者写在专栏文章里的应该是简化了80%的版本。给作者提了个issue看看有什么办法先把简易版本的实现了再向源码进发。（ps：作者是17年毕业的，现在在饿了么工作，比一下感觉自己太弱了...）
- 配了下webpack5，目前还没遇到破坏性变更，体会到了编译速度提升的确挺大。
- 今天看了集英剧（德古拉），结果时间被吞噬了，一个半小时...

### 明

- useAxios简化版本
- ts-axios和ssr-github
- 感觉之前的战线太分散了，这边开一个仓库那边开一个仓库，但是都没怎么捣鼓就停了。准备集中火力，解决掉一个再开始下一个。

## 2020-1-13

### 今

- 今天开开心心的用自己写的API来Mock的时候MongoDB突然崩了...，慌的一批，因为这个东西之前跑了一个多月都没出过问题，难道是哪里边界情况没考虑到？用配置文件重启了Mongod之后就好了。
- 今天主要跟着网课学习，ssr-github的bug修好了，ts-axios也完成了基本功能，到时候还是得去研究下axios源码看看人家node端的实现方式。说到这个，明天研究下node的buffer和流吧，感觉挺重要的。
- 跟着知乎一篇文章写了个[useAxios](https://github.com/linbudu599/Effective-Customize-Hooks/blob/master/hooks/useAxios)，真是鬼才，用 `context` 来实现全局配置，但是这部分今天有点看不懂...
- 整理了闭包到[linbudu599/Penumbra](https://github.com/linbudu599/Penumbra)，不清楚自己是不是真的掌握了？咋会觉得它很简单呢。还有闭包和模块、React组件、Hooks的联系，JS博大精深。
- 开始学webpack5了，做好了全英文开始的准备。

### 明

- webpack5优先，先搞一部分新的东西再整理下新特性
- 继续ssr-github和ts-axios，还剩下好几门网课，移动app、测试、两门小程序（前&后端）
- 再议，根据可用时间灵活安排（真实还没过年就事情一堆）

## 2020-1-12

### 今

- 淦，写hooks的时候发现自己对闭包的理解不够深，于是复习了下闭包...，发现自己之前为啥就是搞不懂闭包呢，明明挺美妙的啊哈哈哈哈哈。顺便把之前的倒计时逻辑也用自定义hooks重写了，[useCountDown](https://github.com/linbudu599/Effective-Customize-Hooks)，这期间又发现了一个在字节工作的大神有个专栏专门介绍自定义hooks，如获至宝！可以安排一哈
- 昨天刚立的flag说可以放一段时间webpack了，今天准备开始看5的时候发现有些地方还是需要琢磨琢磨，再借这个机会配成能开箱即用的模板配置吧。
- 今天的可用时间比较少，ssr-github也只跟进了一小点，出了点奇怪的bug，搜索结果添加筛选条件时会报错，待研究。

### 明

- 专注于研究hooks以及umi

### 明

### 2020-1-11

### 今

- [webpack](https://github.com/linbudu599/Webpack4.x-Template)遗留很久的一个问题突然解决了，感谢umi，使用dev-server-middleware起服务的时候配置项直接引入 `webpack.conf.dev.js` 即可，其中的配置项已经被合并过一次了，不用再在server里合并一次。
- [Log Server](https://github.com/linbudu599/Log_Server)上线了，也接入了天气应用，测试的时候看到成功记录下日志简直不要太开心！但是PM2启动问题还是没法解决，不清楚是配置项有问题还是依赖没装好...
- ts-axios，因为有电子书就跟着电子书敲了，效率高的很，但是担心会不会效果不太好...，想着到时候再全面重构优化一下。君ts当上手

- ssr-github，今天没怎么跟进课程，稍微写了一部分搜索页面，阿西吧又是排序又是限制条件的，但是GitHub竟然api细致到了这种程度...，给劲！
- 一个月前看 `Umi` 文档还一头雾水，但今天就感觉这文档写的真是浅显易懂啊...，我觉得大概可以把 `Umi` 理解成 webpack上层封装 + Next.js式路由 + 强化过的html-webpack-plugin + 一堆灵活的插件。准备这样，写几个demo，fork下社区/官方配置的模板，写个插件，和 `dva`、`antd pro` 搭配，估计四到五天，然后再开始写家园的项目。
- hooks真的好用啊...，今天稍微学习了下优化hooks，不愧是 **hooks哲学**

### 明

> 开始按照重要顺序排序

- （整活）开始写generate天气应用模板的cli了，但是不着急封装成npm，重点是命令行交互一定要骚​
- ts-axios
- ssr-github
- umi-pratice

- 应该这些够了...

## 2020-1-10

### 今

- [webpack](https://github.com/linbudu599/Webpack4.x-Template)的问题解决了，怎么也没想到是 `autoDllPlugin` 的问题，难道是没把dll文件引入好？那这样webpack的配置暂时先告一段落了，现在这个已经可以平时写demo拿来用了。准备开始看webpack5-alpha
- 是真没想到一时心血来潮结果花了好久时间在日志模块上，[半成品](https://github.com/linbudu599/Log_Server)，但是接近五脏俱全了，踩了几个koa和ts搭配的坑，比如声明文件和引入方式啥的，还好很快爬出来了。需要注意下koa把路由分离的方式 `newRouterInstance(server)`，还有就是！PM2和ts的协作有些问题，已经把PM2的解释器配成 `ts-node` 了，但是一直报错，自闭。实在不行在服务器上挂一个终端窗口？这个使用方式（向我自己的域名发起一个POST请求，记录到对应日志）应该还有很大改进空间。
- 还踩了个坑，`Options`请求和跨域，要在koa多配一下对 `options` 请求返回200，不能只配个允许跨域。浏览器级别行为可还行
- 也正是写这个日志服务的时候再次感受到了ts的强大和重要性，于是准备先完成ts实现axios的课程，学完这个我就敢在简历上写自己会ts了吧...
- ssr-GitHub项目，害好讲究啊用户体验，缓存策略啥的，写的有点懵但还是觉得很好玩。

### 明

- 8要留给自己太多任务，万一有个突发情况看着这一堆未完成就心塞
- 开始复盘react？umi&hooks
- ssr-github，搜索模块占了一整章可还行。
- ts-axios，看看能不能把ts之前读文档一直云里雾里的部分解决了，非科班真是有点难...

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
