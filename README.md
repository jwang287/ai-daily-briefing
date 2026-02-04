# AI Daily Briefing - Auto Publisher

自动抓取 AI 新闻，生成简报网站，并部署到 GitHub Pages。

## 功能

- 每日自动抓取最新 AI 新闻
- 生成精美的 HTML 简报
- 推送到 GitHub Pages 免费托管
- 支持历史归档

## 文件结构

```
ai-daily-briefing/
├── index.html          # 主页（最新简报）
├── archive/            # 历史归档
├── data/               # JSON 数据源
├── assets/             # CSS/JS/图片
├── scripts/            # 生成脚本
└── .github/
    └── workflows/      # GitHub Actions
```

## 自动部署

GitHub Actions 每天 UTC 08:00（北京时间 16:00）自动运行：
1. 抓取新闻
2. 生成简报
3. 推送更新
4. 部署 Pages

## 手动触发

```bash
cd scripts
python3 generate_and_push.py
```

## 数据来源

- The Verge AI
- TechCrunch AI
- Hacker News
- ArXiv AI papers

## License

MIT
