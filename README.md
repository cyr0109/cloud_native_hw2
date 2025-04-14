# cloud_native_hw2

## 👤 學生資訊
- **姓名**：陳昱睿  
- **學號**：B11705031
- **GitHub Repo**：[https://github.com/cyr0109/cloud_native_hw2.git](https://github.com/cyr0109/cloud_native_hw2.git)

---

## 📦 Repo 創建與操作過程說明

本次作業我透過 GitHub 網頁介面完成整體操作，以下為詳細步驟說明：

### 1️⃣ 建立 Public Repository
- 登入 GitHub 後，點選右上角「➕」→「New repository」
- 設定 Repository 名稱為 `cloud_native_hw2`
- 選擇 **Public** 權限，以便助教能夠檢視
- 勾選「Initialize this repository with a README」以建立初始的 `README.md`

---

### 2️⃣ 編輯 README.md
- 建立完成後，直接在 GitHub 頁面中點選 `README.md`
- 使用「Edit this file」功能，**加入學號與姓名等個人資訊**，取代原本的預設內容

---

### 3️⃣ 建立分支 `hw1-p` 與 `hw1-f`
- 在 repo 首頁左上角點選「main」旁邊的分支下拉選單
- 輸入 `hw1-p` 並點選「Create branch: hw1-p」
- 重複一次建立 `hw1-f` 分支

---

### 4️⃣ 建立 Issue 與 Issue Template
- 點選「Issues」分頁 →「New issue」建立一個 Open 的 issue
- 回到 Repo 頁面 → 點選「Settings」
- 點選「Set up templates」→ 選擇 Blank → Commit 建立模板

---

### 5️⃣ Pull Request 操作
- 在 GitHub 上切換到 `hw1-p` 分支，新增 `main.py`，點選「Compare & pull request」，建立 PR 對 `main`
- 同樣操作 `hw1-f` 分支，新增並修改 `main.py`，建立 PR
- 在 `hw1-p` 的 PR 中，進入「Files changed」頁籤，**針對程式碼變動留言**

---

### 6️⃣ 設定 GitHub Actions
- 點選「Actions」分頁，選擇建立新的工作流程（Workflow）
- 使用預設模板，並修改為符合作業需求的 `.yml`，**包含至少兩個額外的步驟**
  ```yaml
  - name: List directory
    run: ls -la
  - name: Show time
    run: date
- 在 `hw1-p` 的 PR 中，CI 執行成功 ✅
- 在 `hw1-f` 中的 `blank.yml`，故意加入 `exit 1` 指令讓 CI 失敗 ❌
