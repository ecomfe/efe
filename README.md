
EFE
====

### 简介

百度 EFE(Excellent FrontEnd) 技术体系，前身是 ECOM前端团队，后经过技术的发展，逐渐形成一套完善的前端技术体系。

EFE 技术体系现由多个遵循该技术体系的前端团队所组成。E(Excellent) 代表我们追求卓越的技术态度。

#### 技术委员会

EFE 技术委员会简称 EFE-TC ，由`方向技术负责人`、`团队技术负责人`、`T7+工程师`组成，由 [EFE 主席](chair.md) 带领。

EFE-TC 的主要职责是技术方向把握，在技术上决定 EFE 体系做什么、怎么做、不做什么。

#### 技术方向

EFE技术体系划分了五个技术方向。下面列表中，`@`后面的人为方向负责人。

- Data Visualization @kener
- Interface @Justineo
- Mobile @firede
- Platform @leeight
- RIA @otakustay


### 技术价值观与要求


#### 精细化

- 在技术和方案设计上深思熟虑。应用面越广的技术产品，错误的设计与实现带来的危害和影响面越大。
- 代码质量需要严苛要求，极端情况下因为项目排期紧张导致需要妥协，也应该给出改进时间和计划并严格实施，不得二次拖延。
- 对于问题要明确“做什么（What）”、“为什么（Why）”、“怎么做（How）”，不得以个人经验或者喜好进行技术判断。
- 设计、方案、开发过程需要有记录，便于追溯。
- 无GUI类产品，测试用例需要覆盖完全。有GUI类产品可自由把握。
- 技术产品不允许为了抢占地盘，快速挖坑粗糙实现，然后在不成熟的时候大范围铺开应用。
- 技术产品需要有完善的文档。
- 技术产品需要有使用样例。

#### 开源

业务无关的纯技术产品，必须开源，并且代码托管在github上。包括库、框架、工具等。

纯技术产品的设计、方案选型、开发过程运作需要在github issue上公开、有记录。通过实时聊天工具或邮件达成的技术方案等结论，也需要事后在github issue上记录存档。问题、改进建议等用户反馈，也需要通过github issue进行。


#### 持续性

开源技术产品的维护要有持续性，不得出现找不到人、无人响应的现象。即使技术产品本身已经很完善，github issue中的问题和提议维护者需要持续回答。

当维护者离职时，如果有兴趣可以继续维护，否则需要交接给其他有兴趣的人。


#### 代码符合规范

- JavaScript 代码符合[JavaScript Style Guide](https://github.com/ecomfe/spec/blob/master/javascript-style-guide.md)
- HTML 代码符合[HTML Style Guide](https://github.com/ecomfe/spec/blob/master/html-style-guide.md)
- CSS 代码符合[CSS Style Guide](https://github.com/ecomfe/spec/blob/master/css-style-guide.md)
- LESS 代码符合[LESS Style Guide](https://github.com/ecomfe/spec/blob/master/less-code-style.md)

[fecs](https://github.com/ecomfe/fecs) 工具可以对 JavaScript/HTML/CSS 代码进行检查。


#### 采用模块化方式管理代码

为了便于代码逻辑划分、依赖管理、系统分析与优化，在项目开发中必须使用模块化的方式，各种资源引用不得手工维护。允许使用的模块化方式有以下两种：

1. 通过 [AMD](https://github.com/amdjs/amdjs-api) 进行模块化开发。使用该方式需要遵循[模块规范](https://github.com/ecomfe/spec/blob/master/module.md)
2. 通过 [CommonJS Module](http://wiki.commonjs.org/wiki/Modules/1.1.1) 的方式开发，通过相应工具在开发时与构建时进行前端的运行包装。使用该方式，必须将 CommonJS 模块包装成 AMD。


#### 对同类功能，有复用价值的代码集，通过 package 进行封装

通常在前端项目中，库、框架、多业务共用的公共模块适合通过 package 进行封装。对 package 进行封装需要遵守[包结构规范](https://github.com/ecomfe/spec/blob/master/package.md)，该规范在 [CommonJS Package](http://wiki.commonjs.org/wiki/Packages) 下做了一些细化。

package 可以通过 [private npm](http://edp.baidu.com/) 和 [bower](http://bower.io/) 发布

#### 项目的前端部分，目录结构符合规范

1. 一个只包含前端代码的项目，整个项目必须符合[项目目录结构规范](https://github.com/ecomfe/spec/blob/master/directory.md)。
2. 如果混合PHP、NodeJS等服务端代码的项目，项目的前端部分需要独立单独的目录，该目录的内部结构必须符合[项目目录结构规范](https://github.com/ecomfe/spec/blob/master/directory.md)。


#### 通过同一个blog进行技术输出

对外的技术输出必须统一使用 [EFE Site](http://efe.baidu.com/)。更新方法和内容要求参见 [ecomfe.github.io repos](https://github.com/ecomfe/ecomfe.github.io)

### 加入EFE

加入 EFE 的前端团队，需要符合上述技术价值观和遵循上述要求。

#### 加入方法

1. 联系 EFE 主席，要求加入。可说明加入理由和技术规划或方向。
2. EFE 主席在 EFE-TC 发起讨论和投票。反对票少于 1/3 时，允许加入。

#### 权利

1. 获得至少一个加入 EFE-TC 的名额。
2. 对[标准和规范](https://github.com/ecomfe/spec)发起增补和完善。
3. 影响 EFE 的技术发展方向。
4. 团队所有成员都可以在 [efe.baidu.com](http://efe.baidu.com/) 上增加内容，包括 Blog 文章和技术产品。
5. 以 EFE 的名义进行符合 EFE 价值观与要求的技术的宣传。

#### 义务

1. 遵循上述技术价值观与要求
2. 严格遵守[标准和规范](https://github.com/ecomfe/spec)


### 常见问题

#### EFE 的官方 repos 为啥在 ecomfe org 下？

1. EFE 从 ECOMFE团队(现已解散)发展而来，之前的开源项目很多是放在这的，迁移成本太高。
2. github上，EFE已经被别人先注册了。

#### 团队的开源项目是否必须要放在 ecomfe org 下？

EFE 只要求技术项目必须开源，托管在 github 上，但并不要求必须放在 ecomfe org 下。每个团队都可以有自己的 org，存放自己团队的开源项目。

但是，下面两项资源需要共同维护，不得在自己团队的 org下单独建立：

1. 标准与规范。需要统一使用[EFE spec](https://github.com/ecomfe/spec)
2. Blog.需要统一维护[EFE blog](https://github.com/ecomfe/ecomfe.github.io)



