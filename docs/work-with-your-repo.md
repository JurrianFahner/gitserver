# A practical introduction to git
On the web you can find tons of information about git. In this introduction I will only show how to access your gitserver.

Create a directory and perform git init.
```shell
mkdir somedir
cd somedir
git init
```
Then add your repository to this directory.
```shell
git remote add origin git@gitserver:/opt/git/project.git
```

Create random text files and push the changes to the repostiory.
```shell
echo "file1" > file1.txt
echo "random file2 > file2.txt

git add . 
git commit -m "Comment: init git and added some files"
git push
```

If you want to learn git in a practical way. You might want to consider: https://try.github.io
