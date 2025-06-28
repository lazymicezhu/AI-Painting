# AI 绘画网页（纯 HTML/JS 版）

本项目是一个基于 API 的 AI 绘画网页，使用纯 HTML、CSS 和原生 JavaScript 实现，无需任何前端框架或打包工具。用户可以输入提示词（prompt），可选上传图片，提交后由后端 AI 接口生成图片任务。

## 功能

- 输入提示词生成 AI 绘画任务
- 可选上传图片（文图生图）
- 一键提交，自动调用 API
- 结果以 JSON 格式展示在页面下方
- 支持通过`config.js`灵活配置 API 地址和 Token

## 使用方法

1. **配置 API 参数**
   - 打开`config.js`文件，填写你的 API 地址和 Token，例如：
     ```js
     window.AI_CONFIG = {
       API_URL: "https://api.lazymicezhu.com",
       API_TOKEN: "sk-xxxxxxx",
     };
     ```
2. **打开网页**
   - 用浏览器直接打开`index.html`文件即可使用，无需任何服务器或打包。

## 文件说明

- `index.html`：主网页，包含所有前端逻辑和样式
- `config.js`：API 地址和 Token 配置文件

## 注意事项

- 本项目不会读取`.env`文件，所有 API 参数请在`config.js`中配置
- 结果为 API 返回的原始 JSON 数据，如需展示图片请根据 API 返回内容自行扩展
- 请妥善保管你的 API Token，避免泄露

## 扩展建议

- 可根据 API 返回的图片链接，自动在页面展示图片
- 可增加任务进度轮询、历史记录等功能

---

如有更多需求，欢迎随时提出！
