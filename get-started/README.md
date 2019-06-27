# 关于 NELTS

[Nelts](https://github.com/nelts/nelts) 是一套企业应用级的服务架构，它主要解决 `NODEJS` 在企业应用服务中快速稳定开发以及高[QPS](https://baike.baidu.com/item/QPS)的痛点。它已经帮您完成了绝大多数的前置服务搭建操作，您只要编辑需要的逻辑即可完成服务。同时它也提供常用的一些插件来帮助您扩展功能。它还有一整套完善的脚手架帮助您快速创建模块和快速启动服务。

它与`eggjs`的区别在于：

- [AOP](https://baike.baidu.com/item/AOP/1332219)编程
- 变量作用域隔离，防止全局污染（scoped）。
- 单插件化启动服务。
- 自定义`props`参数向内传递（类似前端的`h(component, props, children)`）。
- 完整的生命周期
- 动态Agents的创建
- 更高QPS的路由设计（基于[Radix Tree](https://en.wikipedia.org/wiki/Radix_tree)算法）

Nelts的简单，可以从以下几步体现。

## 安装脚手架

通过`NPM`来安装：

```bash
$ npm i -g @nelts/cli
```

## 创建第一个项目

通过以下命令来创建一个项目或者一个插件：

```bash
$ nelts init [project]
```

创建出来的模板类似 [https://github.com/nelts/template](https://github.com/nelts/template)

## 调试与发布

- 开发： `npm run dev`
- 编译： `npm run build`
- 启动： `npm run start`
- 重启： `npm run restart`
- 停止： `npm run stop`