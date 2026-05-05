# Git 版本管理实践报告

## 一、学习资料来源
1. Git 官方文档：https://git-scm.com/doc
2. GitHub 官方帮助文档：https://docs.github.com/zh
3. 网络教程：B站 Git 入门视频教程

## 二、实践流程
1.  安装 Git 并完成基础配置（用户名、邮箱）
2.  使用 `git init` 创建本地仓库
3.  编写基础代码文件
4.  完成3次有效提交：
    - 第1次：初始化项目文件
    - 第2次：完善测试代码
    - 第3次：添加 README 实践报告
5.  在 GitHub 创建公开仓库，配置 SSH 公钥
6.  解决 HTTPS 连接问题，改用 SSH 协议完成远程推送

## 三、遇到的问题及解决方法
### 问题1：`error: remote origin already exists`
- 原因：重复添加了同名远程仓库
- 解决：使用 `git remote set-url origin 地址` 直接修改地址，或 `git remote rm origin` 删除后重新添加。

### 问题2：`Recv failure: Connection was reset`
- 原因：国内网络访问 GitHub HTTPS 不稳定，连接被重置
- 解决：删除原有 HTTPS 地址，配置 SSH 公钥，改用 SSH 协议进行推送。

## 四、学习心得
通过本次实践，我掌握了 Git 的基础使用流程，包括仓库创建、提交、远程推送等操作。也理解了版本控制对于代码管理的重要性，以及 SSH 协议在网络不稳定环境下的优势，为后续的项目协作打下了基础。