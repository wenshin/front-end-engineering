# 《Web 前端工程实践指南》前言

在 Web 前端技术发展历史上，出现了几个极大促进前端工程化进程的事件。

1. 2005 年开始 Ajax 技术的快速普及；

2. 2008 年开始，由 Google 引领的 JavaScript 引擎性能快速提升；

3. 2009 年 Ryan Dahl 开发了 NodeJS。

Ajax 的普及和 JavaScript 性能的提升，使得 Web 应用可以在保证用户体验甚至提升用户体验的情况下，通过 JavaScript 实现更复杂的应用逻辑和更庞大的应用规模。业界楷模 Google 最早应用 Ajax 技术开发的邮箱、地图等产品所带来的用户体验的改善和丰富功能，至今仍然让人赞叹不已！

不过当 JavaScript 实现的功能越来越复杂、应用规模越来越庞大时，出现的问题和阻碍也越发的明显。这些问题主要有以下几个方面。

在前端开发生态上，由于浏览器厂商的竞争，以及 CSS、ECMAScript、HTML 等标准的弱约束性。CSS、JavaScript、字体文件格式等糟糕的兼容性一直以来都是前端开发人员非常头痛的问题。为了达到跨浏览器兼容，我们需要做很多处理，并且这些兼容可能很快就会变化，当应用规模庞大了以后，这部分维护成本高的让人怀疑人生！

> 在众多浏览器中，尤以部分 IE 浏览器版本问题最严重，这里借机倡导大家珍爱生命，尽早全面放弃对 IE 10 以下版本的支持。

在应用加载上，Web 1.0 时期，多为文本信息类网站，比如新闻门户等，这时的网页应用的规模较小，网络性能可能造成的白屏时间、页面可交互时间长等问题都还不是很突出。到了 Web 2.0 时期，普通用户在网络上开始大量贡献内容，比如：论坛、博客、社交网站、电商网站等，用户与服务器的交互变得异常频繁起来，功能也格外的丰富。JavaScript、CSS、图片等文件数量和大小都出现了爆发式的增长。虽然网络速度也飞速发展，可是白屏时间和页面可交互时间长的问题却变得更加明显。再到现在的移动 Web 时期，不稳定的网络速度，受限的网络流量，网络性能导致的问题更是关系到企业在竞争中的成败。笔者曾任职的美团之所以在千团大战中胜利，在移动网络下，极佳的页面加载速度带来的良好用户体验是功不可没的（具体的实现方案会在第 6 章中介绍）。针对页面加载速度有研究表明[^1]，网站打开的最佳速度极限是 2 秒，6~8 秒是用户等待极限，超过这个时间范围用户大概率会离你的应用而去。

在开发协作上，早期的开发模式是前后端耦合式的，前端负责页面样式和 JavaScript 逻辑，后端负责页面路由和页面模板动态逻辑实现。在这种模式下，前后端功能联调，Bug 分析等都变得举步为艰，沟通成本非常的高。即使后来，页面模板渲染交由前端开发人员负责，仍然没有太大改善。直到 SPA（Single Page Application 单页应用）和 NodeJS 的出现，前端开发人员可以完全负责包括页面样式、页面路由、页面模板动态逻辑时，才彻底的改善了前后端耦合严重而产生的效率问题。这个发展历程就是前后端分离的历程。

在代码维护上，JavaScript 代码量的增长，传统的全局暴露方法和变量的方式，让应用的质量变得脆弱，同时由于缺乏依赖关系使得代码可读性和可维护性变差。

正是得益于这些问题的出现，前端工程化的需求开始变得迫切。NodeJS 的出现，更是让前端工程化以令人难以置信的速度飞速发展。工程化所需的工具不再需要后端或者前后兼备的人才能开发出来，使用中工具出了问题也更容易解决。

> 这里提到的一些问题只是比较重要的一些问题，当然还有很多其它的问题，比如：CSS 的复用和不可编程问题。

由于前端工程完整的知识内容如海洋般浩瀚，所以本书不得不只围绕常见的可工具化的前端工程技术，通过以问题为指引，带大家熟悉目前前端工程化需要考虑的方方面面，以及时下流行的工程化工具的设计思想和使用。

本书主要分为 6 个部分

1. 第一部分：概述。

第 1 章 软件工程。主要介绍一下软件工程的相关概念、方法论

第 2 章 前端工程。介绍前端工程的发展历程和范围

第 3 章 前端工程师。工程师的素质要求，如何成长为前端工程师

1. 第二部分：工程组织。

第 4 章 项目类型和目录结构

第 5 章 模块化和包管理。JavaScript 模块化、NPM 包管理、CSS 模块化

第 6 章 功能组件化。模块化与组件化的区别、React、Vue.js、Web Component

1. 第三部分：工程技术。介绍需要通过工具进行实现或优化的工程技术

第 7 章 使用 ECMAScript 新特性

第 8 章 可编程 CSS 和局部样式

第 9 章 CSS 兼容技术

第 10 章 文件压缩和合并。JS、CSS、HTML、图片压缩和合并、Base64 编码

第 12 章 内容分发网络（CDN）。

第 12 章 服务器端渲染（SSR）和同构应用。

第 13 章 在线更新（Live Reloading）和热更新（Hot Reloading）。

第 14 章 网络代理。正向代理和反向代理，HTTP/S 代理实现

1. 第四部分：工程质量。

第 15 章 JavaScript 奇怪的地方

第 16 章 TypeScript 和 Flow 的强类型

第 17 章 代码规范和静态检查

第 18 章 自动化测试与 TDD

第 19 章 代码审查（Code Review）

第 20 章 代码重构（Code Refactor）

第 21 章 文档和注释

1. 第五部分：工程效率。

第 22 章 开发环境。IDE和编辑器，Node.js 多版本，脚手架

第 23 章 构建工具。Grunt、Gulp、Webpack、Parcel

第 24 章 Charles 网络代理工具

第 25 章 Node.js 调试工具

第 26 章 便利的 Shell 脚本。Shell 脚本的优势

第 27 章 开发 Node.js 命令行工具

第 28 章 持续集成和自动化部署。Git Hook 和本地集成、Web Hook 和线上集成

1. 第六部分：开发流程和协作。

第 29 章 软件开发模型

第 30 章 需求评审和估时

第 31 章 接口设计和评审

第 32 章 版本和分支管理

第 33 章 部署和发布管理

[^1]: [The Psychology of Web Performance](http://www.websiteoptimization.com/speed/tweak/psychology-web-performance/)

