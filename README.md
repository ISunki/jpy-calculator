<div align="right">
  <strong><a href="#-jpy-salary-converter">English</a> | <a href="#-日元薪资转换器-jpy-salary-converter">简体中文</a></strong>
</div>

---

# 💹 日元薪资转换器 (JPY Salary Converter)

一个极简、优雅且支持 PWA 的纯前端日元薪资计算工具。帮助在日华人或关注日本工作机会的人群，直观地将日元薪资换算为人民币，并掌握不同汇率区间下的真实购买力。

## ✨ 核心功能

* **实时汇率同步**：自动拉取最新的 JPY-CNY 汇率，一键重置恢复实时数据。
* **极简模式切换**：支持输入“税前额面”或“税后到手”，系统自动以 20% 为标准估算税费及社保扣除。
* **全维度计算**：
  * 支持输入年发薪月数，自动计算年薪。
  * 根据 40 小时工作制自动折算时薪。
* **汇率模拟器**：通过拖动滑块或手动输入，自由模拟 3.5 到 5.0 区间内的汇率走向。
* **可视化对比**：内置 Chart.js 柱状图和汇率对照表，直观展示不同汇率下的人民币到手差额。
* **PWA 支持**：可将网页直接“添加到主屏幕”，像原生 App 一样全屏离线使用。
* **深色模式**：原生支持随系统自动切换 Light / Dark Mode。

## 🛠 技术栈

* **纯前端实现**：仅使用 HTML, CSS, JavaScript (Vanilla JS)。无构建工具，开箱即用。
* **Service Worker**：实现静态资源缓存与无网络环境下的离线兜底加载。
* **图表库**：[Chart.js](https://www.chartjs.org/) (CDN 引入)。
* **外部 API**：使用 [ExchangeRate-API](https://www.exchangerate-api.com/) 获取实时汇率。

## 🚀 本地运行与部署

本项目无需复杂的 Node.js 环境或打包流程，只需一台普通的静态服务器即可运行。

1. 克隆本项目：
   ```bash
   git clone https://github.com/ISunki/jpy-calculator.git
