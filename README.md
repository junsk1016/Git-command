git config --global user.name "username"
git config --global user.email "user@email.com"

git config --list
+ 쳐서 user name과 email 이 입력한 내용으로 들어가있는지 확인  

git init
git add .
+ 모든 파일 올리기. 뒤에 .을 붙히면 다 올리겠다는 의미
git statuse
+ add 를 통해 변경된 내용 확인  

git commit -m "first commit"  
+ 내 history에 올리기  

git remote add origin https://github.com/junsk1016/Git-test.git  
+ 내가 새로 만든 깃허브 래퍼지토리에 나오는 git remote add origin "주소"를 복붙하여 연결  

git remote -v  
+ 위에서 입력한 연결이 잘 되었는지 확인하기  

git push origin master  
+ push하기. 하고나서 내가 만든 래퍼지토리 들어가면 생성되어 파일들이 생성되어있음  


내가 파일을 새롭게 추가하고싶으면 git add . 하여 git commit -m "second commit"하고 git push origin master 하면 된다.
