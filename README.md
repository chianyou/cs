# Linux指令
* gzip
  * 壓縮:gzip FileName
  * 解壓縮:
    * gunzip FileName.gz
    * gzip-d FileName.gz
* xz
  * 壓縮:xz-z FileName
  * 解壓縮:xz-d FileName.xz
* tar.gz
  * 壓縮:tar-zcvf FileName.tar.gz DirName
  * 解壓縮:tar-zxvf FileName.tar.gz

# Linux指令-檔案搜索
* find [path] [option] [action] filename
  * option
    * -siz找出大於500M的檔 -size+500M
    * -name
    * -type
    * -user
  * action -exec
    * ls
    * print
* which filename
  * -a:系統會顯示所有被找到的命令執行檔之完整路徑
  * -n<文件名長度>
  * -p<文件名長度>
  * -w:指定輸出欄位的寬度
  * -v:顯示版本訊息
* cat 從第一行顯示檔案內容 形成新檔
  * cat -n file1>file2 把file1的檔案內容加上行號後輸入file2檔案
    * -n 由1開始對所有輸出的行數編號
    * ">" 將多個文件覆蓋到目標文件中
    * ">>" 將多個文件追加到目標文件中 不覆蓋
* tac 從最後一行開始顯示
  * tac-r-s'x\|[^x]' test.log 
    * -r 將分隔符作為基礎正規表達式處理
    * -s 使用string作為分隔符代替默認的換行符
* more 
  * more+20 teatfile 
    * ENTER:向下n行
    * Ctrl+F/SPACE:向下滾動一屏
    * Ctrl+B:返回上一屏
* less 和more類似 顯示檔案是允許用戶既可以向前又可以向後翻頁閱讀檔案
  * ps-ef|less
    * j 下一行
    * k 上一行
    * g 移動到最後一行
* head 取出前面幾行
  * -n
* tail 取出後面幾行
  * -n
  * -n+20: 只列20行以後的資料
  
  
