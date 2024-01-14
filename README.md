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


# プロンプトの表示を変える方法
参考）　bashのプロンプト表示形式を設定する方法　https://zenn.dev/memo/articles/20211004_ps1

PS1で設定可能

\W  現在のディレクトリを表示する　

\w 現在のディレクトリを絶対パスで表示する

\h ホスト名を表示する

\u 現在のユーザー名を表示する


```sh
export PS1="[\W]\$ "
```
