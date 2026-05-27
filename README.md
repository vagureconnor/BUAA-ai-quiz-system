# 《人工智能导论》随机答题系统 🎯

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Platform: Web](https://img.shields.io/badge/Platform-Web-brightgreen.svg)]()
[![Built with: TailwindCSS](https://img.shields.io/badge/Built%20with-TailwindCSS-06B6D4.svg)](https://tailwindcss.com)

一个基于纯前端构建的《人工智能导论》课程模拟刷题与答题系统。界面优雅、响应迅速，支持随机抽题、即时反馈、错题本以及模糊搜索功能，旨在帮助同学们高效复习、攻克期末与阶段性考试。

👉 **[点击立即在线刷题](https://vagureconnor.github.io/BUAA-ai-quiz-system/)** *(请在部署后替换为你的 GitHub Pages 实际链接)*

---

## ✨ 核心特性

- 🎲 **智能随机抽题**：打破固定顺序，全面打牢知识点，告别死记硬背。
- 📝 **双模式切换**：支持标准「答题模式」与随练随查的「背题模式」。
- ❌ **动态错题本**：自动收集答错题目，支持单独强化复习，攻克薄弱环节。
- 🔍 **模糊搜索**：内置全题库模糊检索功能，一键查找特定考点或关键字。
- 📊 **实时统计**：进度条、正确率、已刷题数实时看板，刷题进度了然于心。
- 📱 **完美响应式**：基于 Tailwind CSS 精心设计，无论是电脑、平板还是手机都能获得极致的刷题体验。
- ⚡ **零服务器依赖**：纯 HTML/JS 驱动，数据全部在本地浏览器无缝运行，加载速度极快。

---

## 🛠️ 技术栈

- **Core**: HTML5 / Vanilla JavaScript (ES6+)
- **Styling**: Tailwind CSS (via Play CDN)
- **Design System**: Inter & JetBrains Mono 字体方案，高颜值现代化 UI

---

## 🚀 本地运行与部署

### 本地双击即用
该项目无任何复杂的构建步骤，克隆或下载项目后，**直接双击 `index.html`** 即可在任意浏览器中完美运行。

### 一键部署至 GitHub Pages
如果你想分享给身边的同学在线使用，只需将其发布至 GitHub 并开启 Pages：
1. 将代码推送到你的 GitHub 仓库。
2. 进入仓库的 **Settings > Pages**。
3. 将 **Branch** 设置为 `main` (或 `master`)，点击 **Save**。
4. 稍等片刻即可获得专属的在线刷题网址。

---

## 📖 题库更新与维护

如果你想扩充或修改题库，只需打开 `index.html`，定位到其中的 `questions` 数组，按照以下格式追加或修改对象即可：

```javascript
{
  id: 1,
  type: "single", // 题型：single(单选), multiple(多选), judge(判断)
  question: "这里是题目描述...",
  options: ["选项A", "选项B", "选项C", "选项D"],
  answer: "A", // 答案，多选如 "A,B"
  explanation: "这里是解析（可选）"
}
