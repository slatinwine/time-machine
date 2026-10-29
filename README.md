# 时光机 TIME MACHINE

输入一个日期，穿越回去看看那天——以及历史上每一个「这一天」——发生了什么。

**在线访问（云端 AI 完整版）**：https://time-machine-news.app.workbuddy.host/?sharecode=YMODZSYFLL

## 功能

- **时光穿越**：输入月份+日期（年份选填），返回那天的大事时间线（大事记/出生/逝世）；精确年份命中时以「当日头条」置顶并标注 N 周年
- **AI 主播播报**：把历史事件改写成中文新闻播报，流式逐字输出（WorkBuddy 云端 LLM，免密钥）
- **未来快讯**：输入未来日期，AI 虚构播报那天的新闻（仅供娱乐）
- **微信热文**：微信 24 小时热文榜，点标题直达公众号原文
- **回到今天**：每天 60 秒读懂世界 + 微信热文同屏
- **翻译成中文**：英文史实一键机翻，可切回原文
- **随机穿越**：随机传送到 1900 年以来的某一天

## 后台连通说明

WorkBuddy 云端 AI 有**来源白名单**：仅应用正式域名与 localhost 放行。

| 访问方式 | 历史事件 / 新闻 / 翻译 | 云端 AI 播报 |
|---|---|---|
| WorkBuddy 正式链接 | ✅ | ✅ |
| GitHub Pages | ✅ | ❌（被白名单拦截） |
| 本地打开 index.html | ✅ | ❌ |

GitHub Pages / 本地访问时，AI 播报可在应用内「AI 设置」配置任意 OpenAI 兼容接口（密钥仅存本机浏览器）作为备用；其余功能不受影响。

## 数据来源

- 历史事件：[On This Day API](https://byabbe.se/on-this-day/) / 维基百科（CC BY-SA 3.0）
- 今日新闻：[60s API](https://github.com/vikiboss/60s)
- 微信热文：今日热榜
- 机翻：MyMemory
- 云端 AI：WorkBuddy Cloud LLM（`@tencent-ai/workbuddy-cloud-sdk`，已内联）
