常見指令

####echo
直接輸出字串到terminal
```
huangyuede-MacBook-Pro:note moontea$ echo test5566
test5566
```
加上＄可以輸出已經存在的變數
```
huangyuede-MacBook-Pro:note moontea$ echo $HOME
/Users/moontea
```

####date
查看當前系統時間
```
huangyuede-MacBook-Pro:note moontea$ date
2020年 9月 9日 週三 13時09分15秒 CST
```
按照年-月-日 時：分：秒 查看當前系統時間
```
huangyuede-MacBook-Pro:note moontea$ date "+%Y-%m-%d %H:%M:%S"
2020-09-09 13:11:50
```

####wget

####ps
查看process
|參數|說明|
|:----|:----|
|-a|顯示所有process|
|-u|顯示用戶以及其他資訊|

####top
監視目前process狀態

####kill
關閉process
|參數|說明|
|:----|:----|
|-9|強制關閉process|

####ifconfig
查詢網卡資訊與網路狀態

####free
查詢目前系統的記憶體資訊
|參數|說明|
|:----|:----|
|-h|以M,G等方式顯示數據|

####history
顯示歷史訊息
|參數|說明|
|:----|:----|
|數字|秀出倒數數量的指令|
|-c|清除歷史指令紀錄|

####pwd
顯示當前目錄

####cd
切換目錄
|參數|說明|
|:----|:----|
|-|返回上一次的目錄|
|~|回到家目錄|

####ls
|參數|說明|
|:----|:----|
|-l|查看文件的詳細資料|
|-a|查看所有文件包含隱藏文件|

####cat
查看文件內容
|參數|說明|
|:----|:----|
|-n|查看文件時加上行號|

####more
查看文件內容（用來看內容比較多的）
可以使用空白鍵翻頁

####head
查看文件前10行
|參數|說明|
|:----|:----|
|-n 數字|查看前幾行|

####tail
查看文件後10行
|參數|說明|
|:----|:----|
|-n 數字|查看後幾行|
|-f|持續監看文件內容|

####touch
創建空白文件

####mkdir
創建空白目錄

####cp
用來複製文件或目錄
```
cp 來源文件 目標文件
```
|參數|說明|
|:----|:----|
|-r|遞迴複製（複製目錄）|
|-i|若重複，是否要詢問|

####mv
用來移動文件或重新命名文件
```
mv 來源文件 目標文件
```

####rm
用來刪除文件或是目錄
|參數|說明|
|:----|:----|
|-r|遞迴刪除|
|-f|強制刪除|

####tar
用來進行文件的壓縮或是解壓縮
```
//將/etc下打包成test.tar
tar -cvf test.tar /etc

//將test.tar解壓縮到當前目錄
tar -xvf test.tar

//將test.tar解壓縮到/test
tar -xvf test.tar -C /test
```
|參數|說明|
|:----|:----|
|-c|創建壓縮檔案|
|-x|解開壓縮檔案|
|-v|顯示執行過程|
|-f|目標文件名|
|-z|用Gzip進行|
|-j|用bzip2進行|

####grep
```
//從document.txt找出有keyword的
grep keyword document.txt
```
|參數|說明|
|:----|:----|
|-n|顯示行號|
|-v|去除包含關鍵字以外的行|

####find
尋找文件
```
//找出/etc/目錄下的所有文件
find /etc/*
```
|參數|說明|
|:----|:----|
|-name|搜尋檔名|
|-user|搜尋user|
|-group|搜尋group|