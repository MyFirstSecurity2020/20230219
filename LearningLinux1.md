# 學習更多Linux指令
- linux有許多指令,且不同的linux發行版本有不同的套件軟體
- 底下👍上課會用到
- 參考資料
  - [Linux 命令大全](https://www.runoob.com/linux/linux-command-manual.html)

###  檔案與目錄的基本指令
- ls（list files）: 列出目錄及檔案名
- cd（change directory）：切換目錄
- pwd（print work directory）：顯示目前的目錄
- mkdir（make directory）：創建一個新的目錄
- rmdir（remove directory）：刪除一個空的目錄
- cp（copy file）: 複製檔案或目錄
- rm（remove）: 刪除檔案或目錄
- mv（move file）: 移動檔案與目錄，或修改檔案與目錄的名稱


### {程式|文書}編輯軟體
- 👍gedit
- nano
- vi/vim(高手都愛使用|有一點學習門檻)
  - [精通 vi 與 Vim, 8/e](https://www.tenlong.com.tw/products/9786263243545?list_name=srh)

### 檔案與目錄管理指令
- 
### 檔案壓縮與打包

### 檔案文件處理高階技術 text processing 
- 👍grep: 查找內容包含指定的範本樣式的檔案
  - 如果發現某檔案的內容符合所指定的範本樣式，預設 grep 指令會把含有範本樣式的那一列顯示出來。
  - 範例: strings XXX | grep CTF
  - [Linux 匹配文字 grep 指令用法教學與範例](https://blog.gtwang.org/linux/linux-grep-command-tutorial-examples/)
  - [Linux grep 命令](https://www.runoob.com/linux/linux-comm-grep.html)
- awk: 處理文檔的語言，是一個強大的文本分析工具
  - [Linux awk 命令](https://www.runoob.com/linux/linux-comm-awk.html) 
- sed
  - [Sed Command in Linux/Unix with examples](https://www.geeksforgeeks.org/sed-command-in-linux-unix-with-examples/?ref=leftbar-rightbar) 

### 網路基本指令
- 👍wget
- 👍netstat
- 👍curl

### 行程管理(porcess management)指令
- 你寫的`程式(program)`執行時就成為`行程(porcess)`
- 👍ps:(process status）顯示當前行程的狀態，類似於 windows 的工作管理員。
  - 可以使用ps 指令來尋找正在執行中的處理程序，並顯示這些處理程序的相關資訊。
  - ps -w 顯示加寬(可以顯示較多的資訊)
  - ps -A 列出所有的進程
  - ps -au 顯示較詳細的資訊
  - ps -aux 顯示所有包含其他使用者的行程
  - [Linux ps 命令](https://www.runoob.com/linux/linux-comm-ps.html)
  - [Linux ps command - 20 Real Life Examples](https://www.digitalocean.com/community/tutorials/linux-ps-command)


### 軟體安裝與管理(software package management )
- 不同的linux發行版本有不同的軟體安裝與管理指令
- 常見的有
  - Debian/Ubuntu 系Linux 發行版: apt-get
    - 指令格式 ==>  (sudo) apt-get [命令] [選項] [套件名稱1, 套件名稱2, …]
    - [apt-get 指令一覽](https://b9532026.wordpress.com/2010/03/30/apt-get-%E6%8C%87%E4%BB%A4%E4%B8%80%E8%A6%BD-2/)
    - [[Linux] apt 和 apt-get 之間的差別](https://clay-atlas.com/blog/2021/12/03/linux-apt-get-difference/)
  - RPM Package Manager (RPM)
- Windows作業系統也有不同的軟體安裝與管理指令
  - winget:Windows 封裝管理員(windows10與11內建指令, since 2020) [WIKI說明](https://en.wikipedia.org/wiki/Windows_Package_Manager)
    - 在powershell環境 ~~ 執行 winget install vscode ~~ 就會安裝 Visual Studio Code 微軟開源發布的一款程式碼編輯器
  - Chocolatey .....
