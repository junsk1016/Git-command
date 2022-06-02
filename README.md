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


다른 프로젝트를 같이 할 때는 아래와 같이 한다.  

git clone 하고 뒤에 주소를 입력  

master는 product라고 생각하면 되므로 새로운 branch를 파서 해야 한다.  

git checkout -b junsik
+ junsik이라는 branch를 생성하는 것

이후  
git add .  
git commit -m "second commit"  
까지는 동일하나 push할 때 뒤에 master가 아닌 설정한 브랜치 이름을 넣어야 한다.  
git push origin junsik  

만약 마스터 브랜치에서 업데이트된 소스를 가져올 때는 pull 명령어를 사용한다.  
하지만 pull 하기 전에 꼭 현재 브런치의 소스코드를 commmit을 시켜야 한다.  
git pull origin master  

참고로 브랜치끼리 이동하는 법은 아래와 같다.  

git checkout branch_name  
