# SENTINEL — 安全研究终端

参考终端视频设计的安全研究工作台前端，使用原生 HTML、CSS 和 JavaScript，无需安装依赖。

## 本地查看

下载仓库后双击 `index.html`，或使用独立文件 `SENTINEL-terminal.html`。所有静态资源均为本地文件，无需联网加载字体。

## 功能

- 模拟实时研究日志，支持暂停、继续和清空。
- Claude / GPT / Gemini 三模型协作旁注。
- 示例授权目标与研究任务创建。
- 漏洞队列、优先级筛选、详情及人工复核状态。
- 报告 Markdown、事件日志 JSON 和赏金账本 CSV 导出。
- Ctrl+K 命令面板，支持手机布局。

终端命令：`help`、`status`、`targets`、`findings`、`pause`、`resume`、`clear`、`export`。

## 文件

- `index.html`：页面结构。
- `style.css`：终端风格与响应式样式。
- `app.js`：交互、演示数据与本地状态。
- `SENTINEL-terminal.html`：内嵌 CSS/JS 的独立版本。

## 当前状态

这是可交互的前端原型。所有目标、漏洞、模型连接及金额均为模拟数据，没有连接真实 AI、交易所、扫描器或支付系统，不会进行真实扫描或提交报告。复核状态仅保存在当前浏览器。

已完成桌面端核心交互验证和 390px 手机宽度检查。

上传到仓库不等于已启用网站托管。如需使用 GitHub Pages，可在仓库 Settings → Pages 中选择从 `main` 分支根目录发布。
