# 面试心得

一场好的面试我认为以挖掘候选人的各项能力值深浅为目的，而不是为了“难倒”候选人，所以作为面试官，更多的是去引导、平滑展开考察范围，而不是本着为了面挂候选人的心态去面试。

我认为较差面试体验的情况：
* 去问一些特别偏门或者犄角旮旯的问题，完全不看候选人的过往项目经验或擅长的部分，除非这个岗位真的要求这些非常规技能，否则尽量不要问
* 面试过程很生硬，跳跃性的提问，一会问前端基础，一会突然插了一个毫不相干的问题，前后毫无联系
* “自以为是”，因为即使是面试官也存在知识上的盲区和误区，尽量不要遇到候选人擅长的自己不擅长的就避开了，完全可以是以“请教”的姿态让候选人自己去把一件事情表述清楚，让你都能听懂，也不要过于偏好问自己擅长的但是候选人不擅长的，如果候选人这方面的一些基础问题都没回答出来，就可以换别的了，继续深入没有意义

实际上上面的情况我自己在刚做面试官的时候都犯过，不过人都是会成长的，不断的面试官经历让我知道如何在较短的时间内判断候选人的能力值。其他厂的面试我不太清楚，但一般每一轮的面试考察方向是有区别的，当然也存在一些重叠的部分，我在酷家乐主要负责电话一面、二面笔试、三面，后面可能还会有 1~2 轮的 mgr 面，最后是 hr 面

* 电话面试：主要考察一些基础知识，一些比较容易遇到的实际问题，一些项目经验，可以稍微深挖他擅长的领域，过程中留意一下理解能力、沟通能力，初步判断这个候选人和我们的匹配度，是否可以约到现场面试，不浪费彼此的时间
* 笔试：开场不要直接做题，简短的嘘寒问暖和自我介绍之后，挑一些项目中深度使用、研究的技术，并深入考察，直到他不清楚或达到你考察的目的为止，这时候就可以换一些其他的问题了。然后开始做题，主要考察前端基础、简单的数据结构与算法等，留意一下候选人答题的速度，时间如果太长了建议打断，询问碰到了什么困难，卡在什么地方了，必要时可以做一些提示，如果还是卡住了，那就开始下一个核对答案的环节，这个环节不是仅仅为了一个答案的正确和错误，每道题要询问候选人的解题思路，如果回答比较模糊或过于轻松，建议引申一些相似问题，加大难度考察，直到候选人不清楚或达到你的考察目的
* 三面：能到这一面证明基础能力还是及格的，这一面主要考察项目经验和技术深度、广度、部分的软实力。这一面主要深挖项目的复杂程度和亮眼的地方，考察技术的广度和深度，对业务的理解和思考，对一些实际问题的处理方式和过程，留意沟通协作能力，判断这个人是否有能力 cover 一整个项目并对现有团队起到正向作用，可以考察一些架构、面向对象、设计模式方面的问题，必要时考察一些智力题来判断候选人的聪明程度和反应能力
* mgr 面：省略...主要是结合前面的面试结果综合判断是否可以补位目前团队的人才缺口
* hr 面：谈薪资，软性技能，没有太大毛病一般不会挂掉

以下主要是我在酷家乐作为 web 前端面试官会关心和考察的知识点

## js、nodejs 基础

重点考察的部分，基础不好的建议直接拒了，这块没有太大商量余地

* 闭包
* 作用域
* 原型链
* 变量提升
* 函数参数值传递
* this 指向问题
* 函数提升以及优先级问题
* new 操作符做了什么？
* 用 ES5 实现一个继承（有哪些方式）
* 0.2+0.1不等于0.3问题（浮点数精度）
* 堆、栈、队列是什么？都有什么区别？有什么应用？
* 深拷贝、浅拷贝问题（immutable是怎么实现的？）
* typed array 问题
* es6 箭头函数问题
* let 会提升吗？声明、初始化、赋值等概念。什么是暂时性死区？
* 什么是 iterator？for of 用过吗？
* call、apply、bind 区别，bind 怎么实现的？
* caller、callee 了解吗？什么时候会用到？建议用吗？
* es6 其他特性用过吗？（Class、Map、Set、Decorator 等分别考察）
* promise 实现原理（怎么实现取消？怎么实现 promise all、race 等？）
* async await 知识点（await 的作用，async 返回的是什么）
* generator 又是什么？
* v8 线程模型、event loop（async、promise、nextTick、setTimeout、setImmediate 经典问题变着花样考）
* 进程和线程是什么？有什么区别？
* v8 垃圾回收机制
* 输入 URL，浏览器的执行过程又是怎么样的？（浏览器解析方式、顺序，async、defer等）
* 了解前端模块化吗？有几种规范？（commonjs 和 es module 都是怎么实现的？有啥区别？）

## css、html、dom、浏览器相关基础

没什么好说的，前端必修课，样式、html、浏览器相关的不过关建议直接拒了

* 盒模型
* 样式覆盖优先级问题
* 选择器相关问题
* 怎么解决边距重叠？（什么是 BFC？怎么创建 BFC？）
* flex 弹性布局了解吗？用过哪些？（问一些实际问题）
* 移动端的一些坑
* css modules 了解吗？
* sass、less 用过吗？用到了什么特性？实践情况
* 移动端用什么距离单位？（px、百分比、vw、vh、rem 等）
* 什么是逻辑像素，什么是物理像素，设备像素比又是什么？
* 事件捕获冒泡
* 哪些操作导致 reflow、repaint、composite
* 什么时候用 css 动画，什么时候用 transition？选择标准是什么？（如何知道动画执行结束了？）
* dom api 相关
* cookie、localStorage、sessionStorage 区别和使用场景
* 跨域相关问题，怎么解决？几种方式？
* 缓存相关（强缓存、协商缓存，由此引申 http 相关缓存知识）

## 计算机基础

前端对于协议这块必须是要清晰的，如果是 nodejs 团队建议加大难度

* 前端相关网络知识（tcp，dns，cdn，http，https，http2）
* 安全相关（xss、csrf）
* 怎么实现登录的？（cookie based、session based、jwt）
* https 怎么做到防止数据包被拦截的？
* 证书是什么？
* 几种常见加密算法，对称加密、非对称加密

## 设计模式、架构、编程思想

主要考察架构设计能力，软件工程等基本素质，对于资深前端这块有要求

* 用过什么设计模式？怎么实现的？应用场景？
* 项目是怎么做架构设计的？谈谈你的理解
* mvvm 和 mvc 是什么？有啥区别啊
* 函数式和响应式的理解
* 什么是柯里化，怎么实现柯里化？纯函数是啥？
* defineProperty 用过吗？有什么问题？descriptor 是什么？有哪些属性干嘛用的？initializr 是啥？
* 装饰模式了解吗？装饰器用过吗？哪些场景？（高阶组件、es6 decorator）
* 继承和组合用过吗？什么时候用继承什么时候用组合？（mixin 是什么东西？js 是多继承还是单继承？为什么是单继承？）
* 什么是开闭原则？
* 什么是控制反转？什么是依赖注入？
* 什么是面向切面编程
* 你了解的反模式是什么
* 了解尾调用优化吗？通常用在什么场景？js 引擎有做这层优化吗？什么是尾递归？

## 数据结构、算法相关（easy 难度）

对于前端来说考到 easy 难度差不多了（我自己也是个弱鸡~）

数据结构比如树、链表相关的在前端应用界是常用的，建议考察

图论、动归、线段树、蓄水池抽样等这种根据自己的业务领域来决定是否有必要考察（=. =，web 前端我感觉不需要）

* 大 O 表示法，怎么计算时间复杂度和空间复杂度
* 贪心算法是什么？动态规划是什么？（背包、爬楼梯、金矿问题）
* 实现一个记忆化的斐波那契数列
* 求并集、交集
* 链表相关（排序、合并、去重）
* 树相关（对称二叉树、翻转二叉树、前中后序遍历、深度广度优先遍历、递归非递归实现）

## 智力题

主要考察反应速度、逻辑思维、推理能力，达到正常以上水平即可

* 25 匹马
* 烧绳子
* 推理题

## 应用框架原理

考察是不是只会用，只是技术栈的罗列，而不清楚内部的原理机制，更没有借鉴落地的场景，这块也是重点考察

* react、angular、vue 实现原理（三个选一个候选人最擅长的，针对某个流程详细考察，比如 dom diff、dom patch、脏检查、双向绑定、依赖收集等）
* setState 相关问题，dirty component 是啥
* forceUpdate() 用过吗？是什么干嘛用的？与 setState 有啥区别？
* props 和 state
* 组件设计相关（怎么设计？受控和非受控是什么？）
* children.map 是什么，和普通的 map 有什么区别？使用场景
* cloneElement 干嘛用的，使用场景，和 createElement 区别
* 生命周期相关
* react 16 新特性，react 17 前瞻，fiber，hooks，suspense，异步渲染等
* redux、mobx、vuex、dva 等状态管理框架实现原理，针对几个点详细考察
* redux 或 mobx 怎么处理 side effect？
* redux 中间件模型，thunk 怎么实现？saga 怎么实现的？
* koa、express 用过吗？中间件模型了解吗？有啥区别？
* router 用过吗？核心流程怎么实现的？
* 用过什么 xhr 封装库？（axios、fetch，各家长短？有啥坑吗？）
* babel 原理（有哪些东西，分别干嘛用的，怎么实现的，runtime，polyfill，register）
* webpack 核心流程原理，怎么实现模块化的，treeshaking 怎么做的？

## 其他

随便问点一些业务上的思考，技术加分项，或技术视野、分享、选型方面的考虑

* 使用 typescript 吗？如何看待的，什么情况下用，类型声明文件怎么写的
* 单元测试（jest、mocha、ava）
* 如何发布一个二方或三方包，有哪些考量
* 技术选型的考量指标、维度
* mongo、es、redis 方面相关知识
* 工程化、ci、docker、k8s 相关知识

> 大概就这些，持续更新......








