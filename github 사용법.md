## 깃허브에서 repository를 생성 후 사용법
1. 깃허브에 올릴 디렉토리로 이동 후 '__git init__' 입력하여 저장소 생성
<img width="572" src="https://user-images.githubusercontent.com/32122584/102684618-8226d580-421d-11eb-9774-53a229359506.png">

2. '__git remote add origin [gti url]__' 입력하여 원격저장소를 git에 등록
<img width="355" src="https://user-images.githubusercontent.com/32122584/102684682-404a5f00-421e-11eb-8ed5-e8f19c500eb2.png">
    ex)git remote add origin https://github.com/gone2/study.git

3. 파일을 업로드 하기 위해 '__git add [파일 또는 디렉토리]__ or __[.]__' 입력 (. : 모든 파일을 업로드 하겠다는 뜻)

4. '__git commit -m "업로드 할 파일에 대한 설명"__' 입력

5. '__git push origin master__'를 입력하여 commit 한 것에 대해 저장 (origin : 원격 저장소 주소, master : 현재 브랜치)

## 그 외의 문법
* 원격저장소(github repository)와 로컬저장소(자신의 컴퓨터)의 연결 끊기   
    : '__git remote remove origin__'
    
* 'fatal: remote origin already exists.' 이와 같이 이미 존재한다는 에러가 나타나면 재정의   
    : '__git remote rm origin__'

* git이 추적하지 않는 untracked files을 삭제   
    : 파일을 모두 지우려면 '__git clean -f__'   
        디렉토리까지 모두 지우기 위해서는 '__git clean -fd__'
      
* error: failed to push some refs to 'XXX.git' 이와 같은 에러 발생(: remote와 local 버전이 달라 충돌)   
    : '__git pull origin master__'
