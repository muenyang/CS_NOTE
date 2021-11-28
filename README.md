# CS_NOTE
Linux檔案命名原則、副檔名
區分英文字元的大小寫，基本以小寫為主
檔名長度至多256個字元，可包刮字母、數字、"."(點)、"_"(下劃線)和"-"(連字元)
檔名不可使用的字元："?"(問號),"*"(星號), " "(空格), "$"(貨幣符), "&", 擴號, "/" (斜線)，"." , ".." 
絕對路徑：路徑的寫法『一定由根目錄 / 寫起』，
例如： /usr/share/doc 這個目錄。
相對路徑：路徑的寫法『不是由 / 寫起』，
例如由 /usr/share/doc 要到 /usr/share/man 底下時，寫成： 『cd ../man』，相對路徑意指『相對於目前工作目錄的路徑！』
絕對/相對路徑的移動
cd 	變換目錄
pwd	顯示目前的目錄
mkdir 建立一個新目錄
rmdir 刪除一個裡面是空的空目錄
cp 複製
mv 移動
ls 顯示目錄下的所有內容
cat 查看檔案內容
nano
Ctrl C：顯示游標所在
Ctrl W：查詢命令，按下後會跳轉到末行的反白位置，輸入要查詢的內容在回車及可。

vi/vim(vim相當於vi的升級版)
命令列模式
!=強制
:w 寫入
:q 離開
:set nu 顯示行號，設定後會在每一列的自首顯示該列的行號
:wq
儲存後離開(若為 :wq! 則為強制儲存後離開) 
:w[filename]
將編輯的資料儲存成另一個檔案（類似另存新檔）
:r[filename]
在編輯的資料中，讀入另一個檔案的資料
壓縮檔案
gzip
壓縮：gzip FileName
解壓縮：
gunzip FileName.gz
gzip -d FileName.gz
xz
壓縮：xz -z FileName
解壓縮：xz -d FileName.xz
tar.gz
壓縮：tar -zcvf FileName.tar.gz DirName
解壓縮：tar -zxvf FileName.tar.gz
