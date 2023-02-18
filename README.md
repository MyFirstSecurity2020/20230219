# 20230219 Linux資安技術入門
- 本次課程採用實體資安教學模式以協助學生使用虛擬化技術(在Windows作業系統上安裝Virtualbox,然後匯入linux)學習linux
- 完整的SecurityFoscusOnline2023課程 ~ 請參閱 [完整上課資訊20230211](https://github.com/MyFirstSecurity2020/20230211)
- 實體教學環境
  - 預先作業:本課程使用虛擬機匯入Kali Linux進行教學
  - 步驟1:在你的電腦下載 [virtual box](https://www.virtualbox.org/wiki/Downloads) 並安裝完成 [Virtualbox安裝:YOUTUBE影片](https://youtu.be/FC0CX71aGnc)
  - 步驟2:點選資料下載點, 下載這些龐大的系統
    - Kali Linux [下載點](https://drive.google.com/file/d/1m620Z7KAOSUOLdFH92FYLE2NINb-vJsn/view?usp=sharing)
    - Python會用到的Ubuntu Linux 18.04 LTS(已安裝好pwntools)  [下載點](https://drive.google.com/file/d/1aP-qCFP6jKsGYXtKy9ahwZleQSENEi7C/view?usp=sharing)
  - 步驟3:匯入你要用的linux  [[YOUTUBE教學錄影]](https://youtu.be/GTpQR7fZcwE)
- 學生預先作業:請學生預先申請你的 [github](https://github.com/)  ~ 請上網Google 一下申請辦法

# 上課模式
- 請務必先聽完如何使用本課程與相關規範
- SecurityFoscusOnline2023課程採底下種模式進行:(1)預錄模式 (2)Google Meet線上直播模式 (3)實體資安教學模式
- 此次課程主要採 (3)實體資安教學模式,部分解題採預錄模式(就是錄影後,放在YOUTUBE讓你觀看學習的啦)

# 上課所使用的平台
- [立馬點選加入線上上課平台(Google Meet)上課去]()
  - 8:50開放,9:20關閉連結(遲到太久 ==>就不要參加| 以後會更嚴格: 遲到==>就不要參加)
  - 參與的觀摩教師可自行安排登入時間,也請聯繫小編
- [CTF平台解題(平常沒開放~只有上課期間才會開放)](https://120.114.62.209/)
  - CTF平台會記錄解題的時間,請在上課及開放期間解完你會解的題目
  - 需要做學習歷程的同學,請及早多做準備(先將解題過程使用Windows的剪取工具解貼到你的powerpoint==>後續再加上你的心得)
  - 學習歷程報告盡量強調解題原理,不要只有答案及畫面
  - 平台原則上在上課後當天就會關閉 ==> 你要在兩天內完成會解的題目 ==>請配合時間|不要要求延長賽
  - 燃燒你的資安戰鬥力吧 ! 想想看 CTF戰隊選手兩三天內就要打完戰 你還有時間摸辜錒
  - 專注!專注!再專注!專注的學習 才是 王道!
  - 極限學習的模式:在極短時間內掌握學習主題的深刻內涵 
    - 三天內或三小時把C或C++學會?基本的~ 多深刻? 語法理解 ? 還是 ..就看你的 樓!
- [Discord課程討論區：https://discord.gg/yWCfDtQjzJ 同學互相討論區](https://discord.gg/yWCfDtQjzJ)
  - 嚴格禁止上傳答案(違背者取消證書|且不得參與後續研習活動)
- 上課簽到簿:請每日上課不要遲到
  - [2/11 簽到簿](https://forms.gle/wvuy8prixdNtkY2z9)
  - [2/12 簽到簿](https://forms.gle/zhP9Q5EYPzzRxvB88)
- [問卷調查](https://forms.gle/YUYmUJ16YFjvC8te6)
  - (最後填寫!一定要填寫,不然沒有證書) 
  - 問卷調查須正確填寫CTF註冊的使用者ID 以供驗證解題數作為通過課程考核的依據

# 開場白[[0211課程的錄影]](https://youtu.be/YvQH03hj8mI)
# CTF 入門
- CTF 入門:透過參與CTF搶旗大賽學習資安實務 [線上課程]
  - CTF搶旗大賽
  - 註冊與登入CTF
  - 起手式---文件隱寫術之word隱身術{隱寫術101::STEG1}
    - 另一種解法 請參閱 [如何在Word中快速顯示或隱藏所有隱藏的文本？](https://zh-tw.extendoffice.com/documents/word/906-word-show-hide-hidden-text.html) 
  - 【自行完成】{隱寫術101::STEG2_Secret in PDF}

## Linux資安技術入門 本課程使用Kali Linux進行
- 學習LINUX
  - 使用Google Colab
  - 連線到LINUX CTF去學習
  - 使用線上工具 [Online Linux Terminal](https://www.tutorialspoint.com/linux_terminal_online.php)
  - 使用虛擬機匯入LINUX學習 
- 快速認識Linux作業系統 [線上教材](./Linux/1.基礎linux入門.MD) [[YOUTUBE教學錄影]](https://youtu.be/0T4o81Vghio)
- LINUX指令(commands) == >  Linux 101 + Linux 102
  - [如何透過Windows連線到CTF平台解題](https://github.com/MyFirstSecurity2020/SecurityFoscusOnline2023/blob/main/A2_Linux%E8%B3%87%E5%AE%89%E6%8A%80%E8%A1%93%E5%85%A5%E9%96%80/%E5%A6%82%E4%BD%95%E9%80%8F%E9%81%8EWindows%E9%80%A3%E7%B7%9A%E5%88%B0CTF%E5%B9%B3%E5%8F%B0%E8%A7%A3%E9%A1%8C.md) [[YOUTUBE教學錄影]](https://youtu.be/cULwZeGliuA)
  - Linux指令入門[線上教材](https://github.com/MyFirstSecurity2020/20230211/blob/main/Linux/2_0_.Linux%E5%9F%BA%E6%9C%AC%E6%8C%87%E4%BB%A4.MD)
  - [LINUX CTF 101解答 ](https://github.com/MyFirstSecurity2020/SecurityFoscusOnline2023/blob/main/A2_Linux%E8%B3%87%E5%AE%89%E6%8A%80%E8%A1%93%E5%85%A5%E9%96%80/2_1_Linux101%E8%A7%A3%E7%AD%94.md)  [[Linux1_教學錄影]](https://youtu.be/zLeU0XJAtws)
  - [LINUX CTF 102解答](https://github.com/MyFirstSecurity2020/SecurityFoscusOnline2023/blob/main/A2_Linux%E8%B3%87%E5%AE%89%E6%8A%80%E8%A1%93%E5%85%A5%E9%96%80/2_2_Linux%20102%E8%A7%A3%E7%AD%94.md) 
  - 課後你可以增加國外Linux的練習經驗喔 ~ 完成底下[linux練習](https://overthewire.org/wargames/bandit/) ~ 不會解可以上網參看別人的解法
- 隱寫術(Steganography) == >  隱寫術101
  - 1_認識 隱寫術(Steganography)  [[線上教材]](./Linux/2.%E9%9A%B1%E5%AF%AB%E8%A1%93%E5%85%A5%E9%96%80/1_%E8%AA%8D%E8%AD%98%E9%9A%B1%E5%AF%AB%E8%A1%93%20Steganography.md) [[YOUTUBE教學影片]](https://youtu.be/EJk3l64WPsQ)
  - 2_圖片隱寫術之1:基本入門技_使用linux 基本指令file|strings|grep{隱寫術101::STEG3} [解答](https://github.com/MyFirstSecurity2020/SecurityFoscusOnline2023/blob/main/A2_Linux%E8%B3%87%E5%AE%89%E6%8A%80%E8%A1%93%E5%85%A5%E9%96%80/2.%E9%9A%B1%E5%AF%AB%E8%A1%93%E5%85%A5%E9%96%80/2_%E5%9C%96%E7%89%87%E9%9A%B1%E5%AF%AB%E8%A1%93%E5%9F%BA%E6%9C%AC%E5%85%A5%E9%96%80%E6%8A%80.md) [[YOUTUBE教學影片]](https://youtu.be/farL-eOUXZs)
  - 👍3_圖片隱寫術之2:圖片內嵌`含解答圖片`的解題 
    - 題目:隱寫術101::STEG4  [題目檔案](https://raw.githubusercontent.com/MyFirstSecurity2020/backup/main/steg/steg101/carter.jpg) [解答](https://github.com/MyFirstSecurity2020/SecurityFoscusOnline2023/edit/main/A2_Linux%E8%B3%87%E5%AE%89%E6%8A%80%E8%A1%93%E5%85%A5%E9%96%80/2.%E9%9A%B1%E5%AF%AB%E8%A1%93%E5%85%A5%E9%96%80/3_%E5%9C%96%E7%89%87%E9%9A%B1%E5%AF%AB%E8%A1%93%E4%B9%8B2_%E5%9C%96%E7%89%87%E5%85%A7%E5%B5%8C%E8%A7%A3%E7%AD%94%E5%9C%96%E7%89%87%E7%9A%84%E8%A7%A3%E9%A1%8C.md) [[YOUTUBE教學影片]](https://youtu.be/GLpg4rTmiqg)
  - 4_圖片隱寫術之3:圖片的metadata{隱寫術101::STEG5} [解答](https://github.com/MyFirstSecurity2020/SecurityFoscusOnline2023/blob/main/A2_Linux%E8%B3%87%E5%AE%89%E6%8A%80%E8%A1%93%E5%85%A5%E9%96%80/2.%E9%9A%B1%E5%AF%AB%E8%A1%93%E5%85%A5%E9%96%80/4_%E5%9C%96%E7%89%87%E9%9A%B1%E5%AF%AB%E8%A1%93%E4%B9%8B3_%E5%9C%96%E7%89%87%E7%9A%84metadata.md)
- Linux 鑑識分析入門 == >  Network101
  - 1.鑑識分析與Wireshark入門 [線上教材](./Linux/3_1_鑑識分析與Wireshark入門.md)
  - 2.網路鑑識分析第一步:使用linux指令進行分析[線上教材](./Linux/3_2_網路鑑識分析第一步_使用linux基本指令進行分析.md) [[YOUTUBE教學影片]](https://youtu.be/IL0R7u7W9dk)
    - linux指令: file | strings | grep
    - Network101::NET1
    - Network101::NET2
  - 👍3.HTTP Basic Authentication(認證)封包分析{Network101::NET3} [線上教材](./Linux/3_3_使用wireshark分析HTTPBasicAuthentication.md) [[YOUTUBE教學影片]](https://youtu.be/IH3Q7jdDX5s)
  - 4.HTTP封包分析之檢視出user使用的瀏覽器版本號{Network101::NET4} [線上教材](./Linux/3_4_使用wireshark檢視出user使用的瀏覽器版本號.md) [[YOUYUBE錄影]](https://youtu.be/GnufKfXOSG4)

