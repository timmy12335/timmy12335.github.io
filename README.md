# 前置作業
1. 使用環境：Ｍac M1
2. 安裝homebrew 
  ```
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
  ```
3. 安裝node.js（看個人需求版本）
  ```
    brew install node
  ```
# 建置
1. 安裝Hexo
  - 可以用brew安裝
  ```
    brew install hexo
  ```
  - 或是npm
  ```
    npm install hexo-cli -g
  ```
2. 初始化Hexo
  ```
    hexo init <資料夾名稱>
  ```
3. 於資料夾安裝npm套件
  ```
    # cd 資料夾
    npm install
  ```

# 將內容發佈到GitHub.io
1. 安裝Hexo部署套件
  ```
   # cd 資料夾
   npm install hexo-deployer-git --save
  ```
2. 安裝完成，修改_config.yml中的deploy設定
  ```
    deploy:
      type: git
      repo: https://github.com/{帳號名}/{帳號名}.github.io.git
      branch: master
  ```
3. 執行部署指令
  ```
    hexo deploy
  ```
  後續修改後，可執行以下指令
  ```
    hexo cl // 清除建立的靜態檔案
    hexo g // 建立靜態檔案
    hexo d // 部署
  ```
# 參考網站
- 【學習筆記】如何使用 Hexo + GitHub Pages 架設個人網誌 https://reurl.cc/nOmEaD
- hexo官方網站 https://hexo.io/zh-tw/