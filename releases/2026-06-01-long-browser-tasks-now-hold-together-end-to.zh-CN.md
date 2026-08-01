# 需要操作浏览器的长任务，从头到尾更稳了。

> 内容以官网为准：[https://marsdata.ai/changelog](https://marsdata.ai/changelog)
> 版本 `0.1.1.1828` · 2026-06-01

- **改进** — 长任务、尤其是需要 Mars 帮你操作浏览器的任务（登录某个网站、逐页点击浏览、抓取数据），现在能从头到尾稳定完成了。此前同一个对话有时会在中途被悄悄交接到不同的服务器，导致浏览器里已登录的会话丢失、浏览器任务卡住或失败。现在每个对话都会固定在同一处处理，浏览器会话也会共享，因此浏览器能保持登录状态，在长对话中接着之前的进度继续操作。

---

[返回全部更新](../README.zh-CN.md) · [开始使用 Marsdata AI](https://marsdata.ai) · [English](./2026-06-01-long-browser-tasks-now-hold-together-end-to.md) · [繁體中文](./2026-06-01-long-browser-tasks-now-hold-together-end-to.zh-HK.md)
