# Linux
convenient codes in command line 


## フォルダ内のサブディレクトリを参照して，　フォルダだけを表示
```sh
ls -F $HOME/DirectoryXXX | grep / | sed s/\\/$//g >> SampleList.txt   
```

## サンプルリストを読み込み， 一括処理する
### 1) whileの場合
```sh
cat SampleList.txt | while read line
do

comanndXXXX

done
```

### 2) forの場合
```sh
for a_dir in ${dir_list[@]}; do

comanndXXXX

done

```
