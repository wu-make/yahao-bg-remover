# Yahao - 在线图片去背景终端 🚀

Online background removal tools / websites for removing image backgrounds.（在线图片去背景、去底网站）

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Deploy: GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-blue)](https://wu-make.github.io/yahao-bg-remover/)

**Yahao - 在线图片去背景** 是一个极具赛博朋克（Cyberpunk）风格的纯前端网页工具，致力于为用户提供快速、安全的图像背景剔除服务。

本工具无需注册，无需下载客户端。所有图像处理均依靠您的设备本地算力（浏览器 Canvas API）完成，**图片数据绝对不会被上传至任何云端服务器**，100% 捍卫您的数据隐私。

👉 **[点击此处立即免费使用 Yahao 图片去底工具](https://wu-make.github.io/yahao-bg-remover/)**

---

## ✨ 核心特性

* 🔒 **绝对隐私安全**：无后端服务器架构，断网也能用，你的图片只有你自己能看到。
* 🎨 **自定义色彩剔除**：不仅能去白底、绿幕，支持通过十六进制（HEX）拾色器去除任意背景颜色。
* 🎛️ **实时容差渲染**：拖动滑块即可实时预览去背效果，内置边缘平滑（抗锯齿）算法，拒绝“狗牙”边缘。
* ⚡ **无损极速导出**：一键将处理后的图像导出为保留透明通道（Alpha Channel）的高清 PNG 格式文件。
* 💻 **沉浸式终端 UI**：深度定制的赛博朋克视觉体验，包含 CRT 扫描线、故障文字（Glitch）与发光霓虹特效。

---

## 📖 使用教学（三步搞定）

工具的操作面板位于网页左侧（移动端位于上方），请按照以下步骤操作：

1.  **载入目标图像**
    点击控制台的 **`[ 载入本地图像 ]`** 按钮，从你的电脑或手机中选择一张需要去背景的图片。载入后，右侧面板将显示图像预览。
    
2.  **设定剔除基准与容差**
    * **剔除颜色基准**：点击色块（默认显示为 `#FFFFFF` 纯白），在弹出的颜色选择器中，吸取或选择你要去掉的背景颜色。
    * **算法容差阈值**：左右拖动下方的滑块。向右滑动会扩大颜色的匹配范围（适合背景颜色有渐变或不均匀的图片），向左滑动则收缩匹配范围（能保留更多主体边缘细节）。你可以一边拖动，一边在右侧观察**实时预览**。
    
3.  **导出透明通道图像**
    调整到完美效果后，点击底部亮起的 **`[ 导出透明通道图像 ]`** 按钮，浏览器会自动将去好背景的图片保存为 `.png` 文件到你的设备中。

---

## 🛠️ 技术栈与本地部署

本项目非常轻量化，仅包含单个 `index.html` 文件，没有复杂的依赖关系：
* **HTML5 & Canvas API**：用于图像数据的读取与像素级矩阵运算。
* **Tailwind CSS (CDN)**：用于快速构建响应式原子类样式。
* **Vanilla JavaScript (原生 JS)**：处理前端逻辑与 DOM 交互。

**如果你想在本地运行或二次开发：**
1. 克隆本仓库到本地：
   ```bash
   git clone [https://github.com/wu-make/yahao-bg-remover.git](https://github.com/wu-make/yahao-bg-remover.git)
