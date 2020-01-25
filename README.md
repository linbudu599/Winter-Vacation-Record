# Winter-Vacation-Record

> 我现在觉得，没有什么比坚持记录自己的成长一段时间后再回头感受更有成就感的事情了。

## Focusing On...?

- useAxios（`<GlobalConfig>`、`cancelToken`） :fire:
- 逃避闭包&useRef，why and why not:ambulance:
- 小程序-前端部分👨🏽‍🔧
- GraphQL实践及应用🐣 
- ts-axios单测（jest）

## 2020-1-25

### 今

- 啊...GraphQL的文档属实写的不好，每个知识点就写那么一段没啥意义的代码？？今天用比较粗糙的方式写好了CRUD，但是发现几个地方文档里并没有提到或者提了的示例代码没啥用。重新找了一个大佬做的教程准备明天重新搞以下。感觉这东西学好了用处多多？GitHub的api V4就开始使用GraphQL了，说不定到时候SSR-GitHub也可以用这个版本的API重构下。还剩下几个问题，输入对象类型无法使用，内联片段，拆分查询/操作树等。
- 新开了个记录读源码的库，过程中瞄到了另外一篇挺有意思的文章，埋点方案设计的，感觉挺好玩并且值得整理，就记录到了[Penumbra](https://github.com/linbudu599/Penumbra/blob/master/FE/Track/main.md)里，过程耗时两个小时，各种工具和方案都好奇地试了下。emmm明天开始读Lodash源码整体架构？感谢这些写文章的带哥门
- 小程序的事件机制有点抓瞎，拆分组件的思路很是值得学习！专注于组件自身的事，但又能灵活的被调用~

- 被疫情吓到了，赶紧多买了口罩，YZB标准以上的都被抢完了，害。
- 再尝试了下读useAxios源码，啊啊啊读不进去。明天一早起来读吧

### 明

- 读useAxios
- 写GraphQL
- 写小程序
- 读Lodash
- 写单测
- 美团APP

## 2020-1-24

### 今

- 单测稳定进行，虽然磕磕绊绊的但好歹写的越来越得心应手了。有几个问题还没有解决，关于部分诡异的异步逻辑，还有之前明明感觉天衣无缝的代码竟然跑测试不通过，鬼鬼，果然很有必要搞这个。
- 主要的时间在研究GraphQL，总是想把暂时复杂度不高的逻辑就用高级API来写，结果撞得头破血流呜呜呜我图啥啊，还不是希望以后再写复杂逻辑的时候能得心应手...，比如GraphQLInputObject‘Type，愣是报错，不知道是因为ts的原因没引用正确的泛型还是用的地方错了...koa和ts也有些地方还要研究下。
- 突然发现读源码其实也可以作为一个新线程啊...，和手撕代码写项目并不冲突，还可以当成调剂！明天开始读Lodash源码！
- 给博客配了埋点~

### 明

- 继续跟进现在的任务就好啦，最好开始搞一下react-apollo

## 2020-1-23

### 今

- ts-axios功能至此已经完成（课程部分），后续会再根据官方axios的功能进行扩展，考虑包含Node部分的封装。开始写单测，感觉还挺有意思？？就是边界情况要考虑的真的多诶。而且Jest文档功能一堆，有时间会精读一下选一些可能用得上的功能。
- 练手GraphQL的时候遇到了不少问题，比如MongoDB和TS协作、Koa开启GraphiQL（这个其实百度一下就有，只是我一开始先入为主的去npm上找了），以及GraphQL的Mutation问题。
- 小程序！进展一般，今天没有特别惊艳的收获或者特别烦人的坑。剩余80节课程。

### 明

- MongoDB与TS协作问题！
- 写完大部分单测，或者至少写到50%覆盖率左右
- graphql连接数据库的CRUD
- 小程序预计20节？写一个完整的有交互能力的页面先

## 2020-1-22

### 今

- 啊...，又要开新坑了，准备用graphql+dva+ts+apollo等等写一个todolist，预计会有一次很大的突破，以controller和decorator等语法来写，顺便为nest.js打基础
- 感觉写脚手架要提上日程了，每次都是把之前配好的复制下也太没牌面了，但是现在进度比较赶，再推一推吧...，等到有空了一定要整一个具有牌面的
- ts-axios，重新配一下server，估计要开始写单测了...，cover6、70先将就一下吧
- 小程序，按照每天15~20小节的进度来。今天发现要在小程序里痛痛快快地写原本的代码还真没那么方便，想用async/await还需要专门去拷贝regenerator包里packages/runtime.js这个文件，对版本还有要求，得是0.7左右的，惊了

### 明

- 搭好整个todolist项目结构
- ts-axios/小程序/react-hooks-axios
- 淦，进度真的得加快了，寒假还有读源码这个环节

## 2020-1-21

### 今

- 开始过年了...，往年封建迷信和拜年让我觉得挺好玩的，今年就让我感觉是在浪费大好时光了。主要写了 ts-axios 和继续阅读小程序文档，东西真的还蛮多的。
- 继续学 GraphQL，一时被 Mutation 和 constructing type 搞得有点绕
- useAxios 在看原作者的实现的时候发现 tsx 还有一部分知识需要补一下，于是把原本的自定义 hooks 仓库改成了用于整理写 react 中的经验收集

### 明

- 灵活安排，仍然主要是 GraphQL（Mongoose？）/小程序/useAxios/ts-axios 这几驾马车

## 2020-1-20

### 今

- 新开线程：小程序，评估了一下难度，感觉不是完全崭新的东西，稍微有难度就是 API 和布局啥的了，生命周期的特性我很喜欢，像回到了写 Vue 的青涩年华（？）。预计这门课只需要一周左右，比较有难度的是后面要给茵茵整一个用来记录恋爱琐事防止欠亲亲不给的小程序。
- ts-axios 进度正常，每天写几个 feature，再用自己对 ts 的浅薄认识优化下（我也不知道是不是真的优化了...），看着它一点点完善起来就好兴奋。明天后面的功能就简单得多了，可以补一下几个模块的 doc。
- 开始学 GraphQL，感觉比起 REST 是的确更有优势，无冗余、易维护、要啥就给啥...，得劲！虽然还没学到但是大概有思路后面要怎么在 resolver 里连数据库来进行图式查询了。
- 还是感觉时间不够用，剩下三周左右里还需要完成一个 RN-APP 和一个用于博客的 CMS，以及 Nest 啊 Rx.js 啊等等

### 明

- useAxios，用 ts 推翻重构（跟随原作者思路），全局配置、取消等，从 Umi-hooks 或者 react-use 找几个比较有意义的 hooks 记录等待学习（临幸）
- 跟进小程序、GraphQL、ts-axios

## 2020-1-19

### 今

- 上午主要以 ts-axios 为主，项目庞大之后要弄懂各个功能需要的时间更多了。但是也体会到了用 ts 的好处，不管是 vscode 的强力支持还是各个接口严丝合缝的吻合都有点带劲。
- 复习了一下移动端的知识，包括 JSBridge、Hybrid、rem、vw/vh/vmin/vmax...等等等等，美团 APP 不准备从头到尾跟着视频学了，时间不够。并且这个项目不像 ssr-github 一样那么复杂而且都是新东西，都是已经有不错熟练度的技能如 redux 等。但是准备换一种思路，把它重构一遍，从升级依赖到 tsx 重写，到服务端 RESTFul 等等。应该算个不大不小的挑战。

### 明

- 考虑加一个进程，Blog-CMS 或者小程序。
- 看了一下需要再开始学一门新的东西了，GraphQL/Rx.JS/Immutable.JS/...
- ！忘记非攻老师的公众号还剩一些文章没看完了。

## 2020-1-18

### 今

- 给 hacker-srcipt 提了个[pr](https://github.com/NARKOZ/hacker-scripts/pull/186)，但不是新增语言实现的...，而是很弟弟的把它的 README 翻译了下，虽然应该要很长时间才会收到这个回应（作者好像不咋维护这个仓库了），最近的一个被 close 的 pr 已经是两个月前了。但还是感觉挺有成就感的，或许再过不久我就能给一些开源项目提正经的 PR 了。
- 开始整移动端，感觉好久没写移动端了...JSBridge 啥的都忘光了。准备寒假学两门 APP 开发的课，RN 和 Hybrid。
- ts-axios，今天写了三个 feature，默认配置合并、axios.create()方法扩展、transform 方法实现。准备写完之后看完 axios 源码再继续向着官方完善

### 明

- 为 Penumbra 增添一篇新的文章，[你不知道的 JSON.stringify()](https://github.com/)，学问深的很啊...
- 移动端。（冷漠）

## 2020-1-17

### 今

- ssr-github 完成，但是出现了一个教程里没有的 bug，估计是 GitHub Api 变更了，就像 GitHub OAuth 登陆拿 token 的时候也和视频里的不一样，从对象变成了字符串（字典？）形式，暂时没有处理。

- puppteer 真的好好玩啊，感觉可以用来抢票、爬虫、各种模拟机器人等等，下午花了一个下午的时间研究了几个比较有意思的功能，最后也卡在了一个 bug 上：

  - `evaluate` 方法内无法调用全局函数（模块），即是用 `exposeFucntion` 挂载到 windows 上也是一样...，issues 里有条遇到了和我一样的问题就是用 `exposeFucntion` 解决的，我这是被安排了？

- ts-axios 的配置合并部分，需要的时间超出预期，因此今天没有完成。
- useAxios 重新看和实现了一遍，仍旧没有解决，忐忑不安的把代码都贴给那位前辈了
- 接触了下 feflow，觉得挺简单易上手的，脚手架和构建器知识估计后面写 wss-generator 的时候也可以用上。
- 还是感觉进度偏慢了，觉得自己定位 bug 并迅速解决的能力还有待提升，经常卡在莫名其妙的 bug 上。

### 明

- ssr-github，定位问题并解决
- ts-axios，配置合并、axios.create() 方法扩展
- useAxios，看看作者会不会回复 issue
- 小程序

## 2020-1-16

### 今

- useAxios，作者回复了 issue，但是我今天再看发现估计是我自己的问题，可能又是闭包的锅，准备明天沉下心来再推翻重来。
- ssr-github，issues 界面比我想得难不少...，进度得再推后一到两天，哈哈哈哈想把部署环节当成奖励。今天发现了几个可以再度优化的点：
  - 是否需要把封装过的 `api请求方法` 再封装一层，或者提高原来的封装程度，但这样会不会过于耦合了？
  - 有几个组件感觉还能复用，尤其是拆分成多个文件，但这样可能会影响 `getInitialProps` 或者使得数据流更复杂？需要思考下组件复用的相关思维了
- ts-axios，继续完成了拦截器部分，越来越庞大了整个结构，但是也越来越兴奋了，ts 真的太适合用来写这种复杂应用了。
- dracula，一个新的仓库，主要是之前看了英剧德古拉之后觉得伯爵吸了别人的血就拥有了别人的记忆、能力这点很有意思哈哈哈哈哈。主要突然有这个想法也是因为在群里看到一个学弟自己写的一个 npm 包 [inob](https://github.com/kidonng/inob)，自叹弗如。再次遗憾自己要是大一就进家园就好了。不求像一些神仙一样小学开始学 VB 啥的。

#### 明

- puppeteer，搞一下基本操作，把之前看的那本 ts 入门教程爬下来试试
- feflow 的使用！一直想学一下来的
- 完善 ssr-github 到可部署上线阶段
- ts-axios，跟进到测试部分之前
- h5（孙哥哥的那个仓库）

## 2020-1-15

### 今

- ts-axios 基础工作已经完成，准备开始后续的拦截器、cancelToken 部分，我说 axios 源码怎么有 15k 呢...，这考虑的是真的多。学习到了 typescript 继承内置对象 Error 时需要手动 `Object.setPrototypeOf(this, AxiosError.prototype)` 一下。然后就是觉得这个思路如果让我自己来写起码要有一年工作经验才能写得出来，各处泛型、将类实例和函数结合到一起的思路等等。
- ssr-github 已经接近尾声，剩余 issues 界面的开发，感觉很喜欢这个老师的授课方式，和你一起把坑踩一遍，然后告诉你为啥这是个坑，或者推翻重来告诉你如何提高程序性能（缓存、复用等）。应该会继续完善下去，毕竟 GitHub API 那么完善。如果 next 支持 ts 的话也准备用 ts 重构一下，感觉这个项目还是挺有必要的，各种各样的数据类型、函数重载等。
- 准备开始搞 puppeteer 的时候，被安排的明明白白，因为担心只下 core 可能以后搞大的不够，所以下的完整版，但是一下下了半个小时，所以我就只能孤零零的整个 README 放上学习资源。

### 明

- puppeteer 的基础使用，完成部分功能如爬虫、合并 PDF，考虑基于 puppeteer 写个爬虫工具，React+TS+Koa+MongoDB？再议
- ssr-github，完成、样式调整、撰写文档、测试（暂无）、部署上线，github.linbudu.top
- ts-axios，继续推进
- 准备开始移动端的学习了

## 2020-1-14

### 今

- ssr-github 与 ts-axios 进展顺利，准备给 ts-axios 写下具体的分析文档，作者的思路有点跳跃，需要缓缓。
- useAxios 卡住了，估计不是我的理解问题，去作者源码看了一下，作者写在专栏文章里的应该是简化了 80%的版本。给作者提了个 issue 看看有什么办法先把简易版本的实现了再向源码进发。（ps：作者是 17 年毕业的，现在在饿了么工作，比一下感觉自己太弱了...）
- 配了下 webpack5，目前还没遇到破坏性变更，体会到了编译速度提升的确挺大。
- 今天看了集英剧（德古拉），结果时间被吞噬了，一个半小时...

### 明

- useAxios 简化版本
- ts-axios 和 ssr-github
- 感觉之前的战线太分散了，这边开一个仓库那边开一个仓库，但是都没怎么捣鼓就停了。准备集中火力，解决掉一个再开始下一个。

## 2020-1-13

### 今

- 今天开开心心的用自己写的 API 来 Mock 的时候 MongoDB 突然崩了...，慌的一批，因为这个东西之前跑了一个多月都没出过问题，难道是哪里边界情况没考虑到？用配置文件重启了 Mongod 之后就好了。
- 今天主要跟着网课学习，ssr-github 的 bug 修好了，ts-axios 也完成了基本功能，到时候还是得去研究下 axios 源码看看人家 node 端的实现方式。说到这个，明天研究下 node 的 buffer 和流吧，感觉挺重要的。
- 跟着知乎一篇文章写了个[useAxios](https://github.com/linbudu599/Effective-Customize-Hooks/blob/master/hooks/useAxios)，真是鬼才，用 `context` 来实现全局配置，但是这部分今天有点看不懂...
- 整理了闭包到[linbudu599/Penumbra](https://github.com/linbudu599/Penumbra)，不清楚自己是不是真的掌握了？咋会觉得它很简单呢。还有闭包和模块、React 组件、Hooks 的联系，JS 博大精深。
- 开始学 webpack5 了，做好了全英文开始的准备。

### 明

- webpack5 优先，先搞一部分新的东西再整理下新特性
- 继续 ssr-github 和 ts-axios，还剩下好几门网课，移动 app、测试、两门小程序（前&后端）
- 再议，根据可用时间灵活安排（真实还没过年就事情一堆）

## 2020-1-12

### 今

- 淦，写 hooks 的时候发现自己对闭包的理解不够深，于是复习了下闭包...，发现自己之前为啥就是搞不懂闭包呢，明明挺美妙的啊哈哈哈哈哈。顺便把之前的倒计时逻辑也用自定义 hooks 重写了，[useCountDown](https://github.com/linbudu599/Effective-Customize-Hooks)，这期间又发现了一个在字节工作的大神有个专栏专门介绍自定义 hooks，如获至宝！可以安排一哈
- 昨天刚立的 flag 说可以放一段时间 webpack 了，今天准备开始看 5 的时候发现有些地方还是需要琢磨琢磨，再借这个机会配成能开箱即用的模板配置吧。
- 今天的可用时间比较少，ssr-github 也只跟进了一小点，出了点奇怪的 bug，搜索结果添加筛选条件时会报错，待研究。

### 明

- 专注于研究 hooks 以及 umi

### 明

### 2020-1-11

### 今

- [webpack](https://github.com/linbudu599/Webpack4.x-Template)遗留很久的一个问题突然解决了，感谢 umi，使用 dev-server-middleware 起服务的时候配置项直接引入 `webpack.conf.dev.js` 即可，其中的配置项已经被合并过一次了，不用再在 server 里合并一次。
- [Log Server](https://github.com/linbudu599/Log_Server)上线了，也接入了天气应用，测试的时候看到成功记录下日志简直不要太开心！但是 PM2 启动问题还是没法解决，不清楚是配置项有问题还是依赖没装好...
- ts-axios，因为有电子书就跟着电子书敲了，效率高的很，但是担心会不会效果不太好...，想着到时候再全面重构优化一下。君 ts 当上手

- ssr-github，今天没怎么跟进课程，稍微写了一部分搜索页面，阿西吧又是排序又是限制条件的，但是 GitHub 竟然 api 细致到了这种程度...，给劲！
- 一个月前看 `Umi` 文档还一头雾水，但今天就感觉这文档写的真是浅显易懂啊...，我觉得大概可以把 `Umi` 理解成 webpack 上层封装 + Next.js 式路由 + 强化过的 html-webpack-plugin + 一堆灵活的插件。准备这样，写几个 demo，fork 下社区/官方配置的模板，写个插件，和 `dva`、`antd pro` 搭配，估计四到五天，然后再开始写家园的项目。
- hooks 真的好用啊...，今天稍微学习了下优化 hooks，不愧是 **hooks 哲学**

### 明

> 开始按照重要顺序排序

- （整活）开始写 generate 天气应用模板的 cli 了，但是不着急封装成 npm，重点是命令行交互一定要骚 ​
- ts-axios
- ssr-github
- umi-pratice

- 应该这些够了...

## 2020-1-10

### 今

- [webpack](https://github.com/linbudu599/Webpack4.x-Template)的问题解决了，怎么也没想到是 `autoDllPlugin` 的问题，难道是没把 dll 文件引入好？那这样 webpack 的配置暂时先告一段落了，现在这个已经可以平时写 demo 拿来用了。准备开始看 webpack5-alpha
- 是真没想到一时心血来潮结果花了好久时间在日志模块上，[半成品](https://github.com/linbudu599/Log_Server)，但是接近五脏俱全了，踩了几个 koa 和 ts 搭配的坑，比如声明文件和引入方式啥的，还好很快爬出来了。需要注意下 koa 把路由分离的方式 `newRouterInstance(server)`，还有就是！PM2 和 ts 的协作有些问题，已经把 PM2 的解释器配成 `ts-node` 了，但是一直报错，自闭。实在不行在服务器上挂一个终端窗口？这个使用方式（向我自己的域名发起一个 POST 请求，记录到对应日志）应该还有很大改进空间。
- 还踩了个坑，`Options`请求和跨域，要在 koa 多配一下对 `options` 请求返回 200，不能只配个允许跨域。浏览器级别行为可还行
- 也正是写这个日志服务的时候再次感受到了 ts 的强大和重要性，于是准备先完成 ts 实现 axios 的课程，学完这个我就敢在简历上写自己会 ts 了吧...
- ssr-GitHub 项目，害好讲究啊用户体验，缓存策略啥的，写的有点懵但还是觉得很好玩。

### 明

- 8 要留给自己太多任务，万一有个突发情况看着这一堆未完成就心塞
- 开始复盘 react？umi&hooks
- ssr-github，搜索模块占了一整章可还行。
- ts-axios，看看能不能把 ts 之前读文档一直云里雾里的部分解决了，非科班真是有点难...

## 2020-1-9

### 今

- 继续配[webpack](https://github.com/linbudu599/Webpack4.x-Template)，原本配好了垫片和多页面还是挺带劲的，还配了一个挺好玩的 [webpackbar](https://www.npmjs.com/package/webpackbar)，就是 vuepress 打包的时候会有的那两个进度条，贼有逼格。还有一个[speed-measure-webpack-plugin](https://github.com/stephencookdev/speed-measure-webpack-plugin)，在性能分析上也挺有用的，但是，但是！！全部搞完再优化了一些零碎的配置之后发现出问题了，启动后的页面里明明 js 和 css 文件都被注入了，但是 js 文件并不执行...，用排除法大概锁定范围在了 **optimization.splitChunks** 里，但进一步注释掉有嫌疑的配置项后发现整个模板崩了，js 文件直接不被注入...，淦，我头疼。好像每天都是解决前一天遗留的 :bug:，再留给明天一只更大只的 :bug:
- 看了云谦老师关注的工具，[awesome-f2e-libs](https://github.com/linbudu599/awesome-f2e-libs)，先用的 [**projj**](https://github.com/popomore/projj) 想着管理下项目吧，结果一添加项目就报错，看了下大概一年前就有 issue 提这个问题了，但并没解决...，想着那算了，[**fx**](https://github.com/antonmedv/fx)看起来也不错，可以在命令行打开折叠的 json 对象，好的，`fx data.json` 没反应。打扰了，卑微的 Windows
- [天气小应用](https://github.com/linbudu599/weather-msg-sender)用 ts 重构完了，但是，[那个问题](#2020-1-8)其实算不上被解决了，我最后用的方法是得到返回信息后用 node 写到文件里，然后别的模块再去读取、处理。因为我的思路就是要把异步返回的结果释放到全局里...
- [ssr-github](https://github.com/linbudu599/SSR-Github)，写好首页啦，还是成就感 max 的，突然感觉以后用 ts 重构这个项目不会太简单...，明天继续写仓库详情页啥的。
- 开始学小程序咯~，但是今天就只是开了个头，稍微复习了下文档
- 家园的项目准备再推一下，把 umi、dva、antd pro、react 更深入一些应该会更得心应手

### 明

- 解决 webpack 的 bug，多页面用动态入口配置？
- 继续写 ssr-GitHub、小程序，瞅了一下寒假计划，感觉得再加两个线程了
- [How-to-learn-node-correctly](https://github.com/i5ting/How-to-learn-node-correctly)，写写 node！
- 云谦老师 B 站的 UMI 教程
- 读一读 hooks 相关的文章
- 阮一峰老师的 koa 教程，之前一直想看来着，好像有几个知识点挺重要的
- 新线程：ts 实现 axios
- 新线程：graphql 初体验

## 2020-1-8

### 今

- 继续配置自己的 [`webpack` 模板](https://github.com/linbudu599/Webpack4.x-Template)，主要是 dll 和一些零碎的地方，还剩下**垫片**和**多页面**几个地方没有处理，可能要开始准备看 `webpack5` 的 alpha 了？
- 用 `GitHub Actions` 配好了 CD，先给自己的博客配上了，但是配上之后 nginx 马上崩了，不清楚有没有直接关系，观望一下。主要是感觉 `JenKins` 太折磨了，而且很多功能我远远用不上。
- 新开了个记录 `actions` 的[仓库](https://github.com/linbudu599/Enjoy-Github-Actions)，因为觉得 `GitHub Actions` 还是挺有趣强大的，玩法挺多
- 用 `typescript` 重构了之前的[天气小应用](https://github.com/linbudu599/weather-msg-sender)，同时换了 API 接口（淦，转化逻辑又要重写，原本的那个外国网站崩了..），但是有几个地方卡住了，又是请教大佬又是在思否提问的...
- 继续跟着视频写之前的 [`ssr-github` 项目](https://github.com/linbudu599/SSR-Github)，终于搞懂了代理接口同时区分 csr/ssr 的配置代码...

### 明

- 把那个天气小应用完成好，今天的主要问题是需要得到异步流程结果并且作为模块导出，看了思否大佬的回答大概有思路了
- ssr-github，开始写页面和逻辑
- **家园的项目！** 害我都忘记这一茬了...，验证码的逻辑大概解决了。可能是我写的太远了，需要的接口多了十来个...，后端同学知道估计要鲨了我
- 配完 webpack 剩下的部分
- 写写 node 和 ts
