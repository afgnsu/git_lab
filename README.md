# git_lab
git測試

```
mkdir git_lab #本機建立目錄『git_lab』
cd git_lab
git init #初始化 (建立 .git 目錄)
touch test.rb #建立新的空白檔案『test.rb』
echo '0921380997' > test.rb #在檔案『test.rb』裡加入資料
git add . ＃新增所有檔案到暫存區
git commit -m 'First' #提交儲存並加入說明文字『First』
git push -u origin master #上傳到Github Repo倉庫

git log #查看git操作紀錄
git status #查看git狀態
git branch #查看git分支 (預設只有master)
git checkout -b 0318 #開分支『0318』並切換到分支
touch test2.rb #建立新的空白檔案『test2.rb』
echo '1234' >> test2.rb
git add .
git commit -m 'Second' #提交儲存並加入說明文字『Second』
git checkout master #切回主要『master』
git merge 0318 #合併分支
git branch -d 0318 #刪除分支
git push -u origin master #上傳到Github Repo倉庫

假設這時在Github網頁手動上傳檔案並提交儲存，遠端必須先 pull 再提交
git pull --all
git push -u origin master #上傳到Github Repo倉庫

(105/03/18未完待續)
```
