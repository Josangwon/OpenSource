# 오픈소스 과제
##	깃과 깃허브 관련 용어 조사 및 정리
-------------------
### git 파일의 3가지 상태
  * Committed
    * 데이터가 로컬 데이터베이스에 안전하게 저장되었음
  * Modified
    * 수정했으나 아직 로컬 데이터베이스에 커밋(commit)하지 않은 것
  * Staged
    * 현재 수정한 파일을 곧 커밋 할 것이라고 표시한 상태를 의미
-------------------
### git 디렉토리
  * Working Directory
    * 개발자의 현재 시점으로 소스코드를 수정하며 개발하는 공간
  * Git Directoty
    * 프로젝트의 메타데이터와 객체 데이터베이스를 저장하는 곳
  * Staging Area
    * Working Directory에서 작업한 파일을 Local Repository에 전달하기 위해 파일들을 분류하는 공간
  * Remote Repository
    * 원격 저장소이며 인터넷으로 연결되어 있어 있는 외부 저장소 (웹 페이지에서 보이는 공간)
  * Branch
    * Remote Repository의 현재 상태를 복사하여 master 브랜치와 별개의 작업을 진행할 수 있는 공간
  * Head
    * 현재 작업중인 브랜치의 최근 커밋된 위치
-------------------
### git 기본 명령어
명령어|설명
---|---
git init|저장소 생성
git add {파일1},{파일2}|저장소에 파일 추가
git add --all|저장소에 파일 추가
git commit -m "커밋 메시지"|저장소에 변경 내용 반영
git config|git 설정
git status|저장소 상태 확인
git diff|이전 버전과 비교해 다른 점 나타내기
git log|로그 상태 보기
git push {원격저장소이름} {브랜치이름}|commit한 파일을 원격 저장소에 올림
git fetch {원격저장소이름}|로컬에는 없지만 원격 저장소에 올라가 있는 데이터를 모두 가져옴
git branch {name}|name의 이름으로 새로운 브랜치를 생성
git merge {병합할branch이름}|현재 작업 중인 브랜치에 합칠 커밋을 지정해서 병합
git checkout {name}|현재 브랜치를 name으로 변경
git clone|RemoteRepository에 저장되어 있는 모든 파일들을 Local PC에 복사
git reset{soft/mixed/hard}|작업된 파일들을 특정 커밋 위치로 리셋
