# note-to-svg

將手寫筆記、白板照片或色彩標記草圖，轉換為經確認、系統化、結構化、流程導向的可編輯 SVG。

## 能力

- 辨識文字、顏色、箭頭、空間分組與跨頁關係
- 將內容分為「已確認、合理推測、不清楚」
- 優先詢問會影響架構的歧義
- 建立實體、流程、輸入輸出、角色、驗證關卡與回饋迴圈
- 生成直式、高級科技風格的純向量 SVG
- 在使用者修正語意後，同步更新標籤、連線、圖例與說明

## 安裝

將整個資料夾複製到 Codex 個人 Skills 目錄：

```text
~/.codex/skills/note-to-svg/
```

Windows 範例：

```text
C:\Users\你的帳號\.codex\skills\note-to-svg\
```

## 使用

在 Codex 中輸入：

```text
$note-to-svg
```

並附上筆記圖片及期望的輸出格式。例如：

```text
使用 $note-to-svg，把這些不同顏色標記的手寫筆記整理成直式、流程導向、高級科技風格的 SVG；遇到會影響架構的不確定內容時先向我確認。
```

## 檔案結構

```text
note-to-svg/
├─ SKILL.md
├─ agents/
│  └─ openai.yaml
└─ references/
   └─ svg-guidelines.md
```

