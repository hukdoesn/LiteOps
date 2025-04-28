<div align="center">

# 🚀 LiteOps - 轻量级DevOps平台

<img src="web/src/assets/image/liteops-sidebar.png" alt="LiteOps Logo" width="200"/>

**简单、高效的CI/CD解决方案**

</div>

<p align="center">
  <img src="https://img.shields.io/badge/Vue.js-3-42b883?style=flat-square&logo=vue.js" alt="Vue 3"/>
  <img src="https://img.shields.io/badge/Django-4.2-092e20?style=flat-square&logo=django" alt="Django"/>
  <img src="https://img.shields.io/badge/MySQL-8.0-4479a1?style=flat-square&logo=mysql" alt="MySQL"/>
  <img src="https://img.shields.io/badge/Docker-Ready-2496ed?style=flat-square&logo=docker" alt="Docker"/>
</p>

# 项目介绍

## LiteOps CICD 平台概述

LiteOps是一个实用型的CI/CD平台。它并非追求大而全的DevOps解决方案，而是聚焦于团队日常工作中真正需要的自动化构建、和部署功能，帮助开发团队提高效率，减少重复性工作。

## 项目特点

LiteOps的核心特点是"实用、贴合需求、易于使用"：

- **实用为先**：基于公司现有流程开发，解决实际问题，没有多余花里胡哨功能
- **贴合需求**：针对团队缺少的功能进行定制开发，填补工作流程中的空白
- **易于使用**：简洁直观的界面设计，降低使用门槛，减少学习成本，倾向于Jenkins 自由风格Job

## 项目背景

在日常开发工作中，我发现现有的工作流程存在一些功能缺失。市面上的CI/CD工具虽然功能丰富，但往往存在以下问题：

1. 与公司现有流程不匹配，需要大量定制。比如我公司不允许自动化构建（webhook调用），只允许测试手动构建，便于知道发布之后修改了什么功能/bug。
2. 功能过于复杂，团队实际只需要其中一小部分
3. 学习和维护成本高（Jenkins Pipeline）
4. 难以满足团队特定的自动化需求

LiteOps正是基于这些实际问题开发的，它不追求"高大上"的全面解决方案，而是专注于解决团队日常工作中的实际痛点，提供刚好满足需求的功能。更多的是发布记录功能。如：测试去构建的时候需要去填写构建需求、可观测发布分支最后提交人以及提交commit记录。

## 技术架构

LiteOps采用前后端分离的架构设计：

### 前端技术栈

- **Vue 3**：渐进式JavaScript框架
- **Ant Design Vue 4.x**：基于Vue的UI组件库
- **Axios**：基于Promise的HTTP客户端
- **Vue Router**：Vue官方路由管理器
- **AntV G2**：数据可视化图表库

### 后端技术栈

- **Django 4.2**：Python Web框架
- **Django Channels**：WebSocket支持
- **MySQL 8**：关系型数据库
- **GitPython**：Git操作库
- **Python-GitLab**：GitLab API客户端
- **JWT认证**：用户身份验证

### 部署方案

- **Docker**：容器化部署

## 项目目标

LiteOps的目标是解决团队在开发流程中的实际问题，具体包括：

1. 自动化团队中重复性高的构建和部署工作，节省人力成本
2. 标准化项目的构建流程，减少人为错误
3. 提供清晰的构建状态和日志，方便问题排查
4. 支持团队特有的部署需求，适应现有的服务器环境
5. 简化权限管理

## 适用场景

LiteOps主要适用于以下场景：

- 需要解决特定CI/CD痛点的开发团队
- 现有流程中缺少自动化构建和部署环节的项目
- 希望减少手动操作、提高效率的开发环境
- 对现有工具不满意，需要更贴合实际工作流程的解决方案

## 项目当前状态与未来规划

LiteOps目前处于未完善状态，虽然核心功能已经初步实现，但仍有许多需求和功能有待完善，如实现部署k8s项目。我希望通过开放的方式收集更多的需求和建议，使这个项目能够更好地服务于实际开发场景。

### 需求征集

我诚挚邀请你在查看功能介绍和了解LiteOps后，提供宝贵的意见和建议：

- **功能需求**：你希望看到哪些新功能或改进？
- **用户体验**：界面和操作流程是否符合你的使用习惯？
- **实际场景**：在你的工作环境中，有哪些CI/CD痛点尚未解决？

### 开源计划

在收集并实现足够的功能需求后，能够简单的支持一些团队正常使用，我计划将LiteOps完全开源，让更多的团队能够受益于这个项目。你的每一条建议都将帮助我打造一个更实用、更贴合实际需求的CI/CD工具。


## 📞 联系我

如果您对LiteOps有任何建议、问题或需求，欢迎通过以下方式联系我们：

- **邮箱**：hukdoesn@163.com
- **GitHub Issues**：[提交问题或建议](https://github.com/hukdoesn/liteops/issues)

---