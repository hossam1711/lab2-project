<img width="299" height="169" alt="imgget" src="https://github.com/user-attachments/assets/12eadbee-a72a-4329-8f6b-b5a290fe7b01" />


cd C:\Users\hy\OneDrive\Desktop\prog
git init

git add index.html
git commit -m "Initial commit with index.html"

git branch dev
git branch test
git branch  

git checkout dev
echo "<p>Dev branch changes</p>" >> index.html
git add index.html
git commit -m "Added changes in dev branch"

git checkout test
echo "<p>Test branch changes</p>" >> index.html
git add index.html
git commit -m "Added changes in test branch"

git checkout test
git merge dev

git add index.html
git commit -m "Resolved merge conflict from dev into test"

git remote set-url origin https://github.com/hossam1711/lab2-project.git
git remote -v 

git push -u origin master
git push origin dev
git push origin test

git tag v1.7
git push origin v1.7

git tag v1.8
git push origin v1.8

git tag -d v1.8
git push origin --delete tag v1.8


git add README.md image.png
git commit -m "Added README with image"
git push origin master
