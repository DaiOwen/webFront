1、创建一个新仓库
git clone https://xxxx/yyyy.git
cd yyyy
git switch -c main
touch README.md
git add README.md
git commit -m "add README"
git push -u origin main


2、推送现有文件夹
cd existing_folder
git init --initial-branch=main
git remote add origin https://xxxx/yyyy.git
git add .
git commit -m "Initial commit"
git push -u origin main


3、情况推送现有的 Git 仓库
cd existing_repo
git remote rename origin old-origin
git remote add origin https://xxxx/yyyy.git
git push -u origin --all
git push -u origin --tags
