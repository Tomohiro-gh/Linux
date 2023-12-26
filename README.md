# Linux
convenient codes in command line 


## フォルダ内のサブディレクトリを参照して，　フォルダだけを表示
```
ls -F $HOME/DirectoryXXX | grep / | sed s/\\/$//g >> SampleList.txt   
```

## サンプルリストを読み込み， whileで処理する
```
cat SampleList.txt | while read line
do

comanndXXXX

done
```
