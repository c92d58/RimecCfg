# Rime 配置產生器

> 🎛️ Rime / Squirrel 輸入法配置的視覺化編輯工具，無需手寫 YAML。

🔗 **線上使用：** [rimeccfg.wahsun.org](https://rimeccfg.wahsun.org)

## ✨ 功能

- **輸入方案管理** — 拖曳排序、增刪方案，支援朙月拼音、雙拼等
- **方案切換** — 快捷鍵設定（F4、Ctrl+grave 等）
- **標點符號** — 全形 / 半形對應表編輯
- **按鍵綁定** — 拖曳排序翻頁鍵、編輯鍵
- **翻譯器管線** — 拖曳排序處理器順序
- **詞典編輯器** — 試算表式編輯，支援搜尋、TSV 批量匯入
- **Squirrel 外觀** — 樣式、配色方案、各應用 ASCII 模式
- **YAML 匯入 / 匯出** — 貼上現有配置匯入，下載單檔或全部打包 zip
- **自動儲存** — localStorage 自動儲存，重新整理不丟失

## 🚀 快速開始

1. 打開 [rimeccfg.wahsun.org](https://rimeccfg.wahsun.org)
2. 貼上現有 YAML 配置匯入，或從空白開始
3. 在視覺化介面中調整選項
4. 匯出 YAML，覆蓋 `~/Library/Rime/default.custom.yaml`
5. 點擊鼠鬚管 → **重新部署**

## 🔧 支援平台

| 平台 | 輸入法 |
|------|--------|
| macOS | 鼠鬚管 (Squirrel) |
| Windows | 小狼毫 (Weasel) |
| Linux | ibus-rime / fcitx-rime |

## 📦 技術

純前端單檔案應用，無需構建：

- **js-yaml** — YAML 解析與生成
- **SortableJS** — 拖曳排序
- **JSZip** — 全部配置打包下載
- **Signal Station 主題** — Matrix 綠暗色風格

## 🛠 部署

```bash
# 複製專案
git clone https://github.com/c92d58/RimecCfg.git

# 部署至 Cloudflare Pages
npx wrangler pages deploy . --project-name=rimeccfg --branch=main
```

## 🤝 貢獻

歡迎提交 Issue 與 Pull Request：

1. Fork 本專案
2. 建立分支 (`git checkout -b feature/xxx`)
3. 提交修改 (`git commit -m 'feat: xxx'`)
4. 推送 (`git push origin feature/xxx`)
5. 開 Pull Request

## 📄 授權

MIT License &copy; 2026 WAHSUN

本專案為免費開源軟體，歡迎自由使用、修改與分發。
