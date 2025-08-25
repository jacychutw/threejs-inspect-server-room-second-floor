# 🖥️ threejs-inspect-server-room-second-floor

一個使用 [Three.js](https://threejs.org/) 製作的互動式 3D 專案，  
提供 **第一人稱漫遊**、**碰撞偵測**、**物件標註** 與 **遮擋檢查** 功能，  
讓你可以在虛擬「雙層建築」中自由探索並添加註解。

---

🔍 &nbsp; 查看：<br>
[threejs-inspect-server-room-second-floor](https://jacychutw.github.io/threejs-inspect-server-room-second-floor/)

---

📝 &nbsp; 專案文件：<br>
[Three.js 範例(3)-Two-floors導覽](https://jacychu.medium.com/three-js-%E7%AF%84%E4%BE%8B-3-two-floors%E5%B0%8E%E8%A6%BD-99c193fbcd6f)

---

## ✨ 功能特色
- 🎮 **第一人稱移動**：鍵盤 / 螢幕按鈕控制移動、旋轉、抬頭低頭  
- 🛑 **碰撞偵測**：不可穿牆，模擬真實移動體驗
- 🏃 **Sprint 衝刺**：按住 Shift 可加速移動（快跑），鬆開後回復正常速度
- ⬆️ **多樓層導覽：可在 一樓與二樓 之間自由切換
- 🏷 **標註系統**：點擊物件新增標籤與文字說明
- 💾 **LocalStorage 標註暫存**：標註會依樓層存到 LocalStorage，重新整理後仍可還原(live server)
- 👀 **遮擋判斷**：標籤被物件擋住時自動隱藏  
- 🌐 **Web 部署**：可直接使用 GitHub Pages 預覽

---

## 📷 預覽
<img width="494" height="356" alt="截圖 2025-08-22 下午5 36 22" src="https://github.com/user-attachments/assets/caee3ebb-13b5-4ec7-aaa3-bf30549cc881" />
<img width="494" height="356" alt="截圖 2025-08-22 下午5 36 13" src="https://github.com/user-attachments/assets/7cf27eda-4127-48b9-9dc0-7a42c7c44669" />

---

## 📦 安裝與執行

### 1️⃣ 下載專案
git clone<br>
cd threejs-inspect-server-room－second-floor

### 2️⃣ 啟動本地伺服器
建議使用 VS Code + Live Server 外掛，或用任意靜態伺服器：<br>
npx http-server .
### 3️⃣ 瀏覽器開啟

## 📂 3D 模型來源
本專案的伺服器機房 GLB 檔案來自 Sketchfab<br>
🔗 [Server Room – by BlackIceHUN](https://sketchfab.com/3d-models/server-room-57a480597a20476f9f303fda4a089f86) 
🔗 [A designer meeting room – by AGUNG](https://sketchfab.com/3d-models/a-designer-meeting-room-0f0ff5edb3f8435b87d1c62eda9bc684)

## 🛠 技術細節
Three.js – 3D 場景建立與渲染<br>
GLTFLoader – 載入 .glb 格式模型<br>
CSS2DRenderer – 渲染 2D 標籤（可互動<br>
Raycaster – 用於碰撞偵測與物件點擊選取<br>
自訂樓層管理器 – 處理樓層切換、可見性控制
