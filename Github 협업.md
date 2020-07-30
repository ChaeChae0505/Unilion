# Github 협업 
## 1. 자주쓰는 Git 명령어

|명령어|사용|
|---|---|
|git init|git저장소를 초기화(l)|
|git add.|폴더에 변경된 모든파일 staging area에 올리기(l)|
|git commit-m"커밋에 대한 설명"|유사시 돌아갈 수 있는 저장소의 체크 포인트 생성(l)|
|git remote add origin http://원격 저장소 주소.git|원격저장소(remote repository)연결(l)|
|git branch 브랜치명|새로운 브랜치를 생성(브랜치는 용도에 따라 나누어서 진행)|
|git checkout 브랜치명|해당 브랜치로 이동|
|git push origin 브랜치|원격 저장소의 특정 브랜치에 프로젝트저장|
|git pull origin 브랜치|원격 저장소의 특정 브랜치에서 변경사항 pull해오기|
|git clone http://원격저장소 주소.git|원격저장소에 있는 파일 전체 복사|
|git status|git 저장소의 상태를 확인|
##### (l) 로컬 저장소
![Alt text](/Unilion/1-3.jpg)
<img src="/Unilion/1st/img/together.jpg" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="Github 협업"></img><br/>

## Github와 협업
1) 원격 저장소 생성(Github repository 생성)
2) 팀원을 collaborator로 추가
- Settings > Manage access > invite a collaborator
- 초대 수락
3) 초기 프로젝트 push
* 로컬환경에 올리기
- 초기화 git init 
- 원격저장소 연결 git remote add origin http://원격저장소 주소.git
- 모든 파일 올리기 git add.
- git commit -m "first commit"
- git status : 남아 있는거 확인
* 원격 환경에 올리기
- git push origin master
4) 팀원들의 로컬에 프로젝트 pull
- cd.. 
- mkdir other_user: 다른 팀원이 만든 내용을 가져오기 위해서 폴더 생성
- git clone url

5) 팀원 각자의 브랜치를 생성하여 작업
- git branch : 생성되있는 브런치 확인 할 수 있음 
- git branch other : other이라는 브랜치를 생성
- git checkout other : other 브랜치로 전환가능

6) 브랜치에 작업한 내용을 push
- git add.
- git status
- git commit -m "title change"
- git push origin other

7) Master와 merge하기 전 pull request
- 수정한 사항을 팀원들에게 확인 요청하는 것 
- Pull requests 에서 > 자동으로 확인 해줌 > create pull request

8) Pull request 확인 후 Master와 Merge

## Fork 협업
1) 작업하고 싶은 Repository fork 해오기
- octocat / spoon-knife : github fork 시뮬예제
- 상단에 Fork 버튼 눌러서 가져옴
2) 자신의 로컬에서 작업
- mkdir fork
- cd fork
- git clone url
- ls
- code. : 들어가서 내용수정

3) 변경사항을 자신의 브랜치에 push
- git add.
- git commit -m " id change"
- git checkout -b jungho : 정호라는 브랜치를 바로 만들어 체크아웃 하는 것
- git push origin jungho

4) 원본 레포지토리 소유자에게 pull request 요청
5) 

