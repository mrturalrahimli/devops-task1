git clone git@github.com:mrturalrahimli/devops-task1.git
cd devops-task1 
mkdir Task1
cd Task1
echo 'description'>README.md
cd .. 
git add .
git commit -m 'with comment'
git push origin
git branch dev
git checkout dev
echo 'test file' > testfile.txt
git add .
git commit -m 'added test file'
git push origin dev
git branch trahimli-new_feature
git checkout trahimli-new_feature
echo 'new readme' >README.d
git add .
git commit -m 'comments'
git push origin trahimli-new_feature
git status
echo '.'>.gitignore
git add . 
git commit -m 'added gitignore'
git push origin trahimli-new_feature
git checkout dev
git pull 
git merge trahimli-new_feature
git checkout main
git pull
git merge dev
git status
git checkout trahimli-new_feauture
echo 'edited files' >>README.md
git add .
git commit -m 'edited readme'
git revert HEAD
git checkout main
git log
echo 'pasted log' > log.txt
git add .
git commit -m 'added logs'
git push origin
git branch -d trahimli-new_feature 
