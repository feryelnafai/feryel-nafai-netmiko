# Mon Projet Netmiko

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (main)
$ kdir feryel-nafai-netmiko
bash: kdir: command not found

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (main)
$ cd feryel-nafai-netmiko
bash: cd: feryel-nafai-netmiko: No such file or directory

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (main)
$ mkdir feryel-nafai-netmiko

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (main)
$ cd feryel-nafai-netmiko

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko/feryel-nafai-netmiko (main)
$ cd ..

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (main)
$ ~/Desktop/feryel-nafai-netmiko
bash: /c/Users/DELL/Desktop/feryel-nafai-netmiko: Is a directory

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (main)
$ rm -r feryel-nafai-netmiko

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (main)
$ ~/Desktop/feryel-nafai-netmiko
bash: /c/Users/DELL/Desktop/feryel-nafai-netmiko: Is a directory

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (main)
$ git init
Initialized empty Git repository in C:/Users/DELL/Desktop/feryel-nafai-netmiko/.git/

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ touch README.md

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ echo "# Mon Projet Netmiko" > README.md

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ cat README.md
# Mon Projet Netmiko

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git add README.md
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git commit -m "Ajout du fichier README"
[master (root-commit) ef0a8c8] Ajout du fichier README
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ touch main.py

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ echo 'print("Hello, Git!")' > main.py

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ cat main.py
print("Hello, Git!")

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git add main.py
warning: in the working copy of 'main.py', LF will be replaced by CRLF the next time Git touches it

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git commit -m "Ajout du script Python principal"
[master 7c7f45b] Ajout du script Python principal
 1 file changed, 1 insertion(+)
 create mode 100644 main.py

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git log --oneline
7c7f45b (HEAD -> master) Ajout du script Python principal
ef0a8c8 Ajout du fichier README

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git branch feature/netmiko

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git checkout feature/netmiko
Switched to branch 'feature/netmiko'

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/netmiko)
$
cat main.py
print("Hello, Git!")

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/netmiko)
$

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/netmiko)
$
echo 'def acces_netmiko():
    # Affiche la date coté routeur
    # Affiche les interfaces du routeur dans un fichier interfaces.txt
    print("Connexion au routeur via Netmiko...")

def dire_bonjour():
    print("Hello, Git!")

dire_bonjour()' > main.py

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/netmiko)
$ cat main.py
def acces_netmiko():
    # Affiche la date coté routeur
    # Affiche les interfaces du routeur dans un fichier interfaces.txt
    print("Connexion au routeur via Netmiko...")

def dire_bonjour():
    print("Hello, Git!")

dire_bonjour()

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/netmiko)
$
git add main.py
warning: in the working copy of 'main.py', LF will be replaced by CRLF the next time Git touches it

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/netmiko)
$ git commit -m "Ajout de la fonction acces_netmiko"
[feature/netmiko e0cb63f] Ajout de la fonction acces_netmiko
 1 file changed, 9 insertions(+), 1 deletion(-)

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/netmiko)
$
git checkout master
Switched to branch 'master'

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git branch
  feature/netmiko
* master

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git merge feature/netmiko
Updating 7c7f45b..e0cb63f
Fast-forward
 main.py | 10 +++++++++-
 1 file changed, 9 insertions(+), 1 deletion(-)

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ cat main.py
git log --oneline
def acces_netmiko():
    # Affiche la date coté routeur
    # Affiche les interfaces du routeur dans un fichier interfaces.txt
    print("Connexion au routeur via Netmiko...")

def dire_bonjour():
    print("Hello, Git!")

dire_bonjour()
e0cb63f (HEAD -> master, feature/netmiko) Ajout de la fonction acces_netmiko
7c7f45b Ajout du script Python principal
ef0a8c8 Ajout du fichier README

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git remote add origin https://github.com/feryelnafai/feryel-nafai-netmiko.git

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git remote -v
origin  https://github.com/feryelnafai/feryel-nafai-netmiko.git (fetch)
origin  https://github.com/feryelnafai/feryel-nafai-netmiko.git (push)

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git push -u origin master
info: please complete authentication in your browser...
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 12 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (9/9), 932 bytes | 116.00 KiB/s, done.
Total 9 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/feryelnafai/feryel-nafai-netmiko.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git push -u origin master
branch 'master' set up to track 'origin/master'.
Everything up-to-date

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git push -u origin master
branch 'master' set up to track 'origin/master'.
Everything up-to-date

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git fetch origin

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git checkout -b feature/salut origin/feature/salut
fatal: 'origin/feature/salut' is not a commit and a branch 'feature/salut' cannot be created from it

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ git branch
  feature/netmiko
* master

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ def dire_salut():
    print("Salut, Git!")

dire_salut()
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `"Salut, Git!"'
> cat main.py
bash: syntax error near unexpected token `cat'

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$ cat main.py
def acces_netmiko():
    # Affiche la date coté routeur
    # Affiche les interfaces du routeur dans un fichier interfaces.txt
    print("Connexion au routeur via Netmiko...")

def dire_bonjour():
    print("Hello, Git!")

dire_bonjour()

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (master)
$
git checkout -b feature/salut
Switched to a new branch 'feature/salut'

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/salut)
$ git checkout -b feature/salut
fatal: a branch named 'feature/salut' already exists

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/salut)
$ def dire_salut():
    print("Salut, Git!")

dire_salut()
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `"Salut, Git!"'
>
>
> git fetch origin
bash: syntax error near unexpected token `git'

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/salut)
$ git fetch origin

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/salut)
$ git checkout -b feature/salut origin/feature/salut
fatal: 'origin/feature/salut' is not a commit and a branch 'feature/salut' cannot be created from it

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/salut)
$ def dire_salut():
print("Salut, Git!")
dire_salut()
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `"Salut, Git!"'
>
>
git checkout -b feature/salut origin/feature/salut
bash: syntax error near unexpected token `git'

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/salut)
$ git checkout -b feature/salut origin/feature/salut
fatal: 'origin/feature/salut' is not a commit and a branch 'feature/salut' cannot be created from it

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/salut)
$

git checkout -b feature/salut
fatal: a branch named 'feature/salut' already exists

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/salut)
$ def dire_salut():
print("Salut, Git!")
dire_salut()
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `"Salut, Git!"'
>
>
> def dire_salut():
print("Salut, Git!")
dire_salut()
bash: syntax error near unexpected token `def'
bash: syntax error near unexpected token `"Salut, Git!"'

>
>
>
>
>

def dire_salut():
print("Salut, Git!")
dire_salut()
bash: syntax error near unexpected token `def'
bash: syntax error near unexpected token `"Salut, Git!"'
> 'def' dire_salut():
print("Salut, Git!")
dire_salut()
bash: syntax error near unexpected token `'def''
bash: syntax error near unexpected token `"Salut, Git!"'
> ^[[200~def dire_salut():
bash: syntax error near unexpected token `$'\E[200~def''
dire_salut()
DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/salut)
$ print("Salut, Git!")
bash: syntax error near unexpected token `"Salut, Git!"'

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/salut)
$ dire_salut()
>
>
> def dire_salut():
print(Salut, Git!)
dire_salut()
bash: syntax error near unexpected token `def'
bash: !: event not found
>
>
>
> git push origin feature/salut
bash: syntax error near unexpected token `git'

DELL@DESKTOP-LD9KH7U MINGW64 ~/Desktop/feryel-nafai-netmiko (feature/salut)
$ git push origin feature/salut
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 12 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (9/9), 932 bytes | 77.00 KiB/s, done.
Total 9 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'feature/salut' on GitHub by visiting:
remote:      https://github.com/feryelnafai/feryel-nafai-netmiko/pull/new/feature/salut
remote:
To https://github.com/feryelnafai/feryel-nafai-netmiko.git
 * [new branch]      feature/salut -> feature/salut

