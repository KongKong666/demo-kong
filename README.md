gitd-demo/
 ├── main.go
 ├── go.mod
 └── README.md
package main

import (
    "fmt"
    "os/exec"
)

func main() {
    fmt.Println("🔧 Simple GitD Demo Running...")

    // 运行一个 git 命令测试
    out, err := exec.Command("git", "--version").Output()
    if err != nil {
        fmt.Println("❌ Error running git:", err)
        return
    }
    fmt.Println("✅ Git Version:", string(out))
}
module github.com/你的用户名/gitd-demo

go 1.21
# GitD Demo

A minimal demo project inspired by [codexfield/gitd](https://github.com/codexfield/gitd).

## Run

```bash
go run main.go
git init
git add .
git commit -m "initial demo commit"
git branch -M main
git remote add origin https://github.com/你的用户名/gitd-demo.git
git push -u origin main
# Demo Kong 🦍

> 一个轻量、好玩的示例项目：**一键启动、秒懂结构、方便扩展**。  
> A playful, lightweight demo you can run in minutes and extend easily.

<p align="left">
  <a href="https://github.com/KongKong666/demo-kong/stargazers"><img alt="Stars" src="https://img.shields.io/github/stars/KongKong666/demo-kong?style=flat"></a>
  <a href="https://github.com/KongKong666/demo-kong/issues"><img alt="Issues" src="https://img.shields.io/github/issues/KongKong666/demo-kong"></a>
  <a href="#-license"><img alt="License" src="https://img.shields.io/badge/license-MIT-green"></a>
  <img alt="Made with ❤️" src="https://img.shields.io/badge/made%20with-❤️-ff69b4">
</p>

---

## ✨ 特性 | Features

- 🚀 **一键启动**：本地或 Docker 都可跑
- 🧱 **清晰结构**：规范的目录与脚本
- 🧩 **易扩展**：新增模块/页面不破坏现有代码
- 🔧 **零门槛**：只需要 Node.js 或 Docker 就能玩

---

## 🧪 在线预览（可选）

> 在这里放你的线上地址，或者 GitHub Pages 地址  
> _e.g._ **https://kongkong666.github.io/demo-kong/**

---

## 🛠️ 快速开始 | Quick Start

### 方案 A：Node.js（推荐）
```bash
# 1) 克隆（若已在你仓库里，跳过）
git clone https://github.com/KongKong666/demo-kong.git
cd demo-kong

# 2) 安装依赖（演示用 npm，也可用 pnpm / yarn）
npm install

# 3) 本地启动开发服务
npm run dev

# 4) 生产构建（可选）
npm run build
