# 朵莉姆桌寵

一隻會在 Windows 桌面上生活的點陣桌寵。她是花仙之中、夢境裡的神明——不善言辭、無口、面癱，背上有白色半透明的翅膀。

![動作預覽](動作預覽.png)

> 這是獨立專案，與 [夢境神明像素桌寵](https://github.com/faye910630/dream-god-desktop-pet) 不同。

## 功能

- **8 視圖點陣 + 類 Live2D**：呼吸、頭部擺動、頭髮／裙擺物理、小翅膀拍動
- **桌面生活**：走路、爬視窗、種花、睡覺、跌倒、視線跟著滑鼠
- **照顧**：飽食／清潔／心情／體力；餵白色星星糖、洗澡、睡覺
- **月光花山谷**：雙擊打開照顧面板與對話
- **跳舞／豎琴／布偶**：原創音樂盒舞曲、月光小豎琴、月光兔布偶
- **小遊戲**：雲端之夢、接星星（可接 Unity 建置版）
- **許願**：抬頭看流星
- **開機自動啟動**：右鍵選單可勾選

## 操作

| 動作 | 效果 |
|---|---|
| 點一下 | 摸摸頭（睡著時是叫醒） |
| 拖曳 | 抓起來甩 |
| 雙擊 | 打開「無夢之夢・月光花山谷」 |
| 右鍵 | 餵食、洗澡、睡覺、小遊戲、玩具、開機啟動、關閉 |

## 執行

### 打包版

```powershell
pip install pillow pyinstaller numpy
.\build_l2d_exe.bat
```

輸出在 `dist\朵莉姆桌寵\`：`朵莉姆桌寵.exe` 與 `unity\Build\`（若有建置）。整包複製即可，不需安裝 Python。

### 原始碼版

```powershell
pip install pillow numpy
pythonw l2d_pet.pyw
# 或雙擊 啟動L2D桌寵.bat
```

常用參數：

```powershell
python l2d_pet.pyw --home
python l2d_pet.pyw --do wish
python l2d_pet.pyw --rebuild-sprites
```

存檔：`%APPDATA%\DreamGodL2D\`

## 檔案

- `l2d_pet.pyw`：主程式
- `assets/pixel64/`：64×64 點陣視圖（可直接改）
- `assets/icons/moonflower.ico`：月光花圖示
- `assets/six_views/`：多視圖與 Live2D 拆件素材
- `fonts/Cubic_11.ttf`：俐方體 11 號（SIL OFL）
- `unity/DreamGodGames/`：Unity 6 小遊戲專案
- `build_l2d_exe.bat`：打包 exe

## 角色

朵莉姆為原創角色，角色設計版權歸作者所有。
