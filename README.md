# git_lab  
![Git Help](https://github.com/afgnsu/git_lab/blob/master/git_help.png)  
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

git stash #儲藏
git reflog #追蹤變更軌跡

tree .git
git cat-file -p c545efebe5f57d4cab2ba9ec294c4b0cadf672

(105/03/18未完待續)
```

![DEMO](https://github.com/afgnsu/git_lab/blob/master/DEMO.png)  
![DEMO2](https://github.com/afgnsu/git_lab/blob/master/DEMO2.png)  
[連猴子都學的會Git](https://backlogtool.com/git-guide/tw/)  
[儲藏](https://git-scm.com/book/zh-tw/v1/Git-%E5%B7%A5%E5%85%B7-%E5%84%B2%E8%97%8F-Stashing)  
[追蹤變更軌跡](https://github.com/doggy8088/Learn-Git-in-30-days/blob/master/docs/16%20%E5%96%84%E7%94%A8%E7%89%88%E6%9C%AC%E6%97%A5%E8%AA%8C%20git%20reflog%20%E8%BF%BD%E8%B9%A4%E8%AE%8A%E6%9B%B4%E8%BB%8C%E8%B7%A1.markdown)  
