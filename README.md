<!-- TOC -->

- [基于 React 的组件库](#基于-react-的组件库)
    - [Workspaces(工作区) + lerna](#workspaces工作区--lerna)
        - [Workspaces](#workspaces)
    - [参考](#参考)

<!-- /TOC -->

# 基于 React 的组件库

## Workspaces(工作区) + lerna

解决的痛点：

1. 新建项目需要重新配置各种工具，且各项目间依赖的版本管理千头万绪，难以统一管理

2. 通过 npm/yarn link 虽然可以实现本地依赖，但依旧不够自动化

3. eslint，babel 等配置项无法实现多项目共享

### Workspaces

> 工作空间是一种新的方式来设置您的包体系结构，默认情况下可以从Yarn 1.0开始。它允许您以这种方式设置多个软件包，只需要运行yarn install一次即可将所有软件包安装在一个通道中。

workspaces 字段的使用前提必须是 private 为 true 到的项目下，否则会抛出如下错误：

```
Workspaces can only be enabled in private projects.
```

## 参考

[yarn workspaces](https://yarnpkg.com/lang/en/docs/workspaces/)