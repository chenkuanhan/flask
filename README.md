# 快速開始


```Python
# pip install flask

from flask import Flask

app = Flask(__name__) # 定義一個 Flask 物件 = app 
                      # 基於 app Flask 物件進行不同的設定跟操作
                      # 例如：路由、樣板 ...

@app.route("/") # 當收到網址 `/` 請求時，進入這個路由
def hello_world():
    return "<p>Hello, World!</p>"

```
```Python
'''
pip install flask
pip install Flask

'''



from flask import Flask,request

app = Flask(__name__) 

# 接收請求（HTTP Request）
@app.route("/",methods=['GET','POST']) 
def hello_world(): 
  name = request.args.get("name")
  name = request.form.get("name")
  return "<p>hello.html</p>"
  



```
# cheat sheet
**建立existing repository(local repository)同樣也一定是從README.md檔案開始**

![螢幕擷取畫面 2024-06-08 124629](https://github.com/chenkuanhan/flask/assets/104495841/1060c502-f51f-4f88-9dd1-84c8e1fab60e)













## memo
1. copy .venv file
2. copy .git file
## 比較
5. flask --app app run
6. flask run
7. python -m flask --app <filename> run
```
Windows PowerShell
著作權（C） Microsoft Corporation。保留擁有權利。

安裝最新的 PowerShell 以取得新功能和改進功能！https://aka.ms/PSWindows

PS C:\Users\Asus> cd C:\Users\Asus\Documents\clone_repo
PS C:\Users\Asus\Documents\clone_repo> git clone https://github.com/chenkuanhan/ignore_try2.git
Cloning into 'ignore_try2'...
remote: Enumerating objects: 11, done.
remote: Counting objects: 100% (11/11), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 11 (delta 1), reused 11 (delta 1), pack-reused 0
Receiving objects: 100% (11/11), done.
Resolving deltas: 100% (1/1), done.
PS C:\Users\Asus\Documents\clone_repo> git clone https://github.com/chenkuanhan/flask.git
Cloning into 'flask'...
remote: Enumerating objects: 1532, done.
remote: Counting objects: 100% (1532/1532), done.
remote: Compressing objects: 100% (1438/1438), done.
remote: Total 1532 (delta 87), reused 1506 (delta 78), pack-reused 0
Receiving objects: 100% (1532/1532), 6.27 MiB | 6.31 MiB/s, done.
Resolving deltas: 100% (87/87), done.
PS C:\Users\Asus\Documents\clone_repo> start .
PS C:\Users\Asus\Documents\clone_repo> cd C:\Users\Asus\Documents\integration\web
PS C:\Users\Asus\Documents\integration\web> git status
fatal: not a git repository (or any of the parent directories): .git
PS C:\Users\Asus\Documents\integration\web> ls

    目錄: C:\Users\Asus\Documents\integration\web

Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        2024/6/8  下午 01:14             17 .gitignore
-a----        2024/6/8  下午 01:11            556 README.md

PS C:\Users\Asus\Documents\integration\web> git init
Initialized empty Git repository in C:/Users/Asus/Documents/integration/web/.git/
PS C:\Users\Asus\Documents\integration\web> git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Asus\Documents\integration\web> git remote -v
PS C:\Users\Asus\Documents\integration\web> git add .
PS C:\Users\Asus\Documents\integration\web> git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

PS C:\Users\Asus\Documents\integration\web> git commit -m "first commit"
[master (root-commit) a2a90bf] first commit
 1 file changed, 25 insertions(+)
 create mode 100644 README.md
PS C:\Users\Asus\Documents\integration\web> git status
On branch master
nothing to commit, working tree clean
PS C:\Users\Asus\Documents\integration\web> git log
commit a2a90bf669f679180e3e8c41cb8a521eefdb4cfd (HEAD -> master)
Author: Hank <kuanc1784@gmail.com>
Date:   Sat Jun 8 13:19:08 2024 +0800

    first commit
PS C:\Users\Asus\Documents\integration\web> git remote -v
PS C:\Users\Asus\Documents\integration\web> git remote add origin https://github.com/chenkuanhan/readme_try.git
PS C:\Users\Asus\Documents\integration\web> git remote -v
origin  https://github.com/chenkuanhan/readme_try.git (fetch)
origin  https://github.com/chenkuanhan/readme_try.git (push)
PS C:\Users\Asus\Documents\integration\web> git push origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 20 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 634 bytes | 634.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/chenkuanhan/readme_try.git
 * [new branch]      master -> master
PS C:\Users\Asus\Documents\integration\web>

```
