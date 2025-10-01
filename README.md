# 打卡系統

極簡風格的打卡與工作日誌系統

## 功能特色

- ⏰ 即時台灣時間顯示
- 👆 上下班打卡
- 📝 每日三件重要事項追蹤
- 📊 進度視覺化（橘色/綠色進度條）
- 💾 自動儲存到 Supabase
- 📥 Excel 匯出功能
- ☁️ 自動週報（每週五 18:00）

## 技術棧

- **前端**: React 18
- **資料庫**: Supabase (PostgreSQL)
- **自動化**: n8n workflows
- **部署**: Zeabur

## 開始使用

直接開啟 `index.html` 即可使用

## 部署到 Zeabur

1. 連接此 GitHub repository
2. 選擇 Static Website
3. 自動部署完成

## 環境設定

需要設定以下服務：

1. **Supabase**: 資料庫
   - 建立三個資料表：attendance, work_logs, daily_tasks
   - 設定 RLS policies

2. **n8n**: Workflow 自動化
   - Workflow 1: 資料匯出服務
   - Workflow 2: 自動週報排程
