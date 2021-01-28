# Info_Git for me
* for md: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#images

## Table of Contents [TOC]
This is for git-test.

## git command
1.
```
echo "# git_test" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/greym00n/git_test.git
git push -u origin master
```
- refer(kor): https://blog.naver.com/ljy9378/221376435078
- refer2: https://gist.github.com/davfre/8313299
- refer3: https://education.github.com/git-cheat-sheet-education.pdf


2.
```
git add .
git commit -m "name what you want"
git push -u origin master
```

3.
```
git fetch origin
git pull
```

4.
```
git config credential.helper store
```
put the command to input id/pw
```
git fetch

git config --global credential.helper 'cache --timeout 7200'
```
1 day - 86400
7 days - 604800
30 days - 2592000

- refer(kor): https://webisfree.com/2017-05-19/git-%EC%95%84%EC%9D%B4%EB%94%94-%ED%8C%A8%EC%8A%A4%EC%9B%8C%EB%93%9C-%EC%9E%85%EB%A0%A5-%EC%95%88%ED%95%98%EB%8A%94-%EB%B0%A9%EB%B2%95

5.
```
git remote rm origin
```
it yeilds 'usage: git remote remove <name>' msg.
then do whatever you wanted to do.
 
- refer(kor): https://blog.naver.com/whatadayy/221846393216

6.
```
git status

git commit -am "commit contents"

```
- refer: https://blog.naver.com/youjin020257/221820300094

7. force to pull
```
git reset --hard HEAD
git pull
```
or
```
git fetch --all
git reset --hard origin/master
git pull origin master
```
- refer: https://www.hahwul.com/2016/04/07/coding-git-pull-pull/
- refer2: https://www.hahwul.com/2016/04/07/coding-git-pull-pull/

8. How to set webhook
- refer: https://gist.github.com/eslachance/40ac1c8232a5a019b43ee3f588d637ad


9. initialize

Command line instructions
You can also upload existing files from your computer using the instructions below.


Git global setup
```
git config --global user.name "Chijung"
git config --global user.email "chijung.jung@gmail.com"
```

Create a new repository
```
git clone https://gitlab.com/Chijung/project_spinner.git
cd project_spinner
touch README.md
git add README.md
git commit -m "add README"
git push -u origin master
```

Push an existing folder
```
cd existing_folder
git init
git remote add origin https://gitlab.com/Chijung/project_spinner.git
git add .
git commit -m "Initial commit"
git push -u origin master
```

Push an existing Git repository
```
cd existing_repo
git remote rename origin old-origin
git remote add origin https://gitlab.com/Chijung/project_spinner.git
git push -u origin --all
git push -u origin --tags
```


10. helpful source

https://stackoverflow.com/questions/13716658/how-to-delete-all-commit-history-in-github
https://stackoverflow.com/questions/44563131/removing-contributor-from-github-com
https://stackoverflow.com/questions/11868447/how-can-i-remove-an-entry-in-global-configuration-with-git-config
