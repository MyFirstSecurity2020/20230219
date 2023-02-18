# 學習更多Linux指令
- linux有許多指令,且不同的linux發行版本有不同的套件軟體
- 底下👍上課會用到
- 參考資料
  - [Linux 命令大全](https://www.runoob.com/linux/linux-command-manual.html)

###  👍檔案與目錄的基本指令 [Linux 文件与目录管理](https://www.runoob.com/linux/linux-file-content-manage.html)
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

### 檔案壓縮與打包
- 👍tar 
  - 副檔名是`.tar` (僅打包，無壓縮)
  - 副檔名是`.tar.gz` (打包+壓縮)
  - 解壓縮並解包最常見指令 ==>  tar -xzvf test.tar.gz
  - -z或--gzip或--ungzip ==> 通過gzip指令處理備份檔案
  - -x或--extract或--get ==> 從備份檔案中還原檔案
  - [[Linux] .tar .tar.gz 常用壓縮打包指令 (打包、壓縮、解壓縮)](https://richarlin.tw/blog/linux-tar/)
  - [Linux tar 命令](https://www.runoob.com/linux/linux-comm-tar.html)
  - [tar command in Linux with examples](https://www.geeksforgeeks.org/tar-command-linux-examples/)
- gzip(壓縮檔案) vs gunzip(解壓縮檔案) :  - 副檔名是 `.gz` 
  - 指令格式: gzip `FileName(檔案名稱)` ==> 產生 FileName.gz
  - 解壓縮檔案 == > gunzip FileName.gz 或是  gzip `-d` FileName.gz
- zip(壓縮檔案) vs  unzip(解壓縮檔案) : 副檔名是 `.zip` 

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
  - `語法格式Syntax`: wget [option參數選項] [URL網址]
  - [Linux 使用 wget 指令自動下載網頁檔案教學與範例](https://blog.gtwang.org/linux/linux-wget-command-download-web-pages-and-files-tutorial-examples/) 
  - [Wget command in Linux/Unix](https://www.geeksforgeeks.org/wget-command-in-linux-unix/)
  - [Wget Command in Linux with Examples](https://linuxize.com/post/wget-command-examples/)
- 👍netstat ==> 列出網路連線的各種資訊
  - 範例: netstat -ano
    - 列出所有連接埠（Port） ==> `-a`
    - 不要解析 DNS ==> `-n`
    - Displays active TCP connections and includes the process ID (PID) for each connection. ==> `-o`
  - [使用 Netstat 指令檢測網路的技巧](https://blog.gtwang.org/linux/linux-netstat-command-examples/) 
- 👍curl:強大的命令列瀏覽器
- 👍nc:強大的網路連線  ==> 超強 的socat 指令
  - [Netcat（Linux nc 指令）網路管理者工具實用範例](https://blog.gtwang.org/linux/linux-utility-netcat-examples/) 
  - [Linunx 指令 nc 用法](https://myapollo.com.tw/zh-tw/linux-command-nc/)
  - [Linux nc command](https://www.computerhope.com/unix/nc.htm)
  - [The socat Command in Linux](https://www.baeldung.com/linux/socat-command#:~:text=Socat%20is%20a%20flexible%2C%20multi,%2C%20TCP%2C%20or%20standard%20input.)
  - [Getting started with socat, a multipurpose relay tool for Linux](https://www.redhat.com/sysadmin/getting-started-socat)
- 連線到遠端伺服器 telnet(不安全)  vs ssh(安全)
  - 範例 ==> ssh `-p 2200` lab@120.114.62.111 
  - [Linux 的 SSH 安全加密連線指令使用教學、設定檔配置範例](https://blog.gtwang.org/linux/ssh-command-tutorial-and-script-examples/) 
- ping: 檢測主機。
  - 執行 ping 指令會使用 ICMP 傳輸協定，發出要求回應的資訊
  - 若遠端主機的網路功能沒有問題，就會回應該資訊，因而得知該主機運作正常。
  - ping -c 4 www.google.com   [手動終止==> Ctrl+C]
  - [Linux ping 命令](https://www.runoob.com/linux/linux-comm-ping.html)
- traceroute   [WINDOWS作業系統也有tracert] tracert www.google.com
  - 從你的電腦到google 經過多少router(路由器) ==>traceroute www.google.com [有很多節點不會顯示 是因為關掉ICMP] 
  - [Linux traceroute命令](https://www.runoob.com/linux/linux-comm-traceroute.html)

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
- procinfo(process information):顯示系統狀態
  - 從/proc目錄裡讀取相關資料，將資料妥善整理過後輸出到標準輸出設備。
  - [Linux procinfo命令](https://www.runoob.com/linux/linux-comm-procinfo.html) 
- kill :刪除執行中的程式(行程)或工作。
  - [Linux kill命令](https://www.runoob.com/linux/linux-comm-kill.html) 

### 軟體安裝與管理(software package management )
- 不同的linux發行版本有不同的軟體安裝與管理指令
- 常見的有
  - Debian/Ubuntu 系Linux 發行版: `apt(Advanced Packaging Tool)` | apt-get
    - 指令格式 ==>  (sudo) apt-get [命令] [選項] [套件名稱1, 套件名稱2, …]
    - [apt-get 指令一覽](https://b9532026.wordpress.com/2010/03/30/apt-get-%E6%8C%87%E4%BB%A4%E4%B8%80%E8%A6%BD-2/)
    - [[Linux] apt 和 apt-get 之間的差別](https://clay-atlas.com/blog/2021/12/03/linux-apt-get-difference/)
    - [Linux apt 命令](https://www.runoob.com/linux/linux-comm-apt.html)
  - RedHat: Yum( Yellow dog Updater, Modified) | RPM Package Manager (RPM)
    - 基於 RPM 套件管理，能夠從指定的伺服器自動下載 RPM 包並且安裝
    - 可以自動處理依賴性關係，並且一次安裝所有依賴的套裝軟體，無須繁瑣地一次次下載、安裝。
    - yum 提供了查找、安裝、刪除某一個、一組甚至全部套裝軟體的命令，而且命令簡潔而又好記。
    - [Linux yum 命令](https://www.runoob.com/linux/linux-yum.html)
- Windows作業系統也有不同的軟體安裝與管理指令
  - winget:Windows 封裝管理員(windows10與11內建指令, since 2020) [WIKI說明](https://en.wikipedia.org/wiki/Windows_Package_Manager)
    - 在powershell環境 ~~ 執行 winget install vscode ~~ 就會安裝 Visual Studio Code 微軟開源發布的一款程式碼編輯器
  - Chocolatey .....

### 使用者(user)管理 |群組(group)管理

