# github_connect
git을 통해서  github와 연결할 수 있다

## 1. 🍎[깃설치](https://git-scm.com/download/win)

git에 올려야 할 폴더에 가서 shift+우클릭하여  이름이 Powershell 창열기
   
   git init(깃 초기화시키기)
   
      -.git폴더가 생성됨  
      
 
----------------------------
## 2.깃 설치후 git bash 열기

![image](https://user-images.githubusercontent.com/129706762/235417894-3ae93a07-1c03-45c1-991b-2faaea5774f9.png)
   유저 이메일 설정하기 (반드시 git hub에 가입했던 이메일 주소와 동일해야한다. 이름은 상관없음)

    $ git config --global user.name "jaeyoung"
    
    $ git config --global user.email "jykkim01@naver.com"

내 정보 확인하기

git config--list

##  ⬆️위의 연결은 해당 컴퓨터에서 한번만 실행하면 됨
---------------------------------------------------

#github에 코드 업로드하기

🍎 *초기화작업

  git init
 
🍎 *추가할파일 (폴더 안의 내용을 모두 올림)

     git add .
     
🍎 *히스토리 만들기(-m은 메세지를 의미함 ""의 안에는 히스토리 이름을 적음)

 git commit -m "first commit"
 
🍎 *github의 repository를 만들고 그 주소와 연결하기

          git remote add origin https://github.com/jaejae87/css_flex.git
          
🍎*연결이 잘 됬는지 확인하기

    git remote -v

🍎*github에 올리기

git push origin master
----------------------------------
## 수정하여 다시 업로드 할때

11.파일위치 찾기  dir로 찾음
22.파일 찾으면 기존의 자식으로 cd 자식이름 
최종까지 찾으면 그 자리에서 git in 시작!!!

#1. 기존의 코드를 다운받는 행위를 해야한다. 

     git pull origin master

#2.다시 push해야 한다.

    git push origin master

