# Zhi Grip

**知握：语音驱动的视觉抓取智能机械臂**

**第一届浙江省大学生人工智能竞赛** 揭榜挂帅赛题四（智能制造场景智能检测及无序分拣）**一等奖** （省级 A 类）

---

## Language / 文档语言

[English](./Readme_en.md) / [中文](./Readme.md)

---

## 项目介绍

### 目录结构

```bash
.
├── 3DParts            # 3D 结构模型文件
├── Control            # Arduino 嵌入式控制模块
├── Controller         # 上位机控制模块
├── Joystick           # 手柄控制模块
├── xiaozhi-server     # 语音交互服务器（小智）
├── docs               # 文档资源
├── LICENSE            # 开源许可证（GPL3.0）
└── Readme.md          # 项目说明文档
````

### 项目架构

整体架构如下所示：

![架构图](./docs/poster.png)

### 视频演示

点击下图查看演示视频：

[![视频截图](./docs/img1.jpg)](https://www.bilibili.com/video/BV1MnWhzCEoF/)

---

## 快速上手

### 克隆项目

本项目使用了 Git 子模块，推荐使用以下方式克隆：

```bash
# 一次性克隆主仓库及所有子模块
git clone --recursive https://github.com/LanternCX/ZhiGrip.git
```

如果你已克隆仓库，但子模块未初始化或未更新，可执行：

```bash
git submodule update --init --recursive
```

### 更新所有 Git 子模块

当子模块仓库有更新时，可以在主项目中同步所有子模块：

```bash
# 拉取主仓库最新更新
git pull origin main

# 更新所有子模块到最新版本
git submodule update --recursive --remote
```

这样可以确保主项目引用的所有子模块均为最新状态。

## 许可证与贡献

### 使用本代码

使用本项目代码请遵守 **GNU General Public License v3.0 (GPL-3.0)** 协议。

使用或修改本代码时，请遵循 GPL-3.0 的条款，并在分发时附带相同许可证。

使用本代码或有合作or疑问，欢迎发邮件交流：caoxin@xysu.tech

### 提交贡献

如果你希望贡献代码到子模块，请按以下流程操作：

1. 在 GitHub 上 **Fork** 对应的子模块仓库，例如 `Control` 或 `xiaozhi-server`。

2. 克隆你 Fork 的子模块到本地：

```bash
git clone https://github.com/<你的用户名>/<子模块仓库>.git
cd <子模块仓库>
```

3. 创建新的分支进行开发：

```bash
git checkout -b feature/your-feature-name
```

4. 完成开发后提交代码：

```bash
git commit -m "feat: 描述你的改动，遵守 Angular Git commit 规范"
```

5. 推送分支到你 Fork 的仓库：

```bash
git push origin feature/your-feature-name
```

6. 在 GitHub 上对子模块仓库发起 **Pull Request（PR）**

   注意：PR 是针对子模块仓库，而不是主仓库。

## 其他文档

1. [初赛报告](./docs/Report.md)
2. [机械臂运动学解算](https://www.caoxin.xyz/index.php/archives/50/)
3. [PPT](https://www.canva.cn/design/DAG6yuzZL9I/euldDkP9Nv4h0vfzjcehqg/edit?utm_content=DAG6yuzZL9I&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)