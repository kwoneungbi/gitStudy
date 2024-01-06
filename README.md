# 📂 git 기본 명령어

> GitHub는 개발할때 협업할 수 있도록 지원하는 플랫폼이다.
> 주로 버전관리 및 코드 공유에 사용되며, Git이라는 버전 관리 시스템을 기반으로 한다.
> 오늘은 기본적인 명령어들에 대해 공부해 보려고한다.

### 1) git clone [URL]

<br> GitHub에서 프로젝트를 로컬 컴퓨터로 복사한다.![](https://velog.velcdn.com/images/eungbi/post/b27a25f2-3010-4f1b-8dfc-f33a5422f68d/image.png)

### 2) git add [파일명]

<br> 변경된 파일을 스테이징 영역에 추가한다.
![](https://velog.velcdn.com/images/eungbi/post/4e1b7585-be03-4de5-b062-d4919690dbc8/image.png)<br>git add .은 모든 변경된 파일을 스테이징 영역에 추가한다는 의미이다.![](https://velog.velcdn.com/images/eungbi/post/e279ffd5-5f0c-4f2e-95a1-14b123fcf049/image.png)

### 3) git commit -m "[커밋 메시지]"

<br> 스테이징 영역의 변경사항을 로컬 저장소에 저장한다.
![](https://velog.velcdn.com/images/eungbi/post/acf03fd1-a666-4081-b39c-f008f3acabf2/image.png)<br>git commit과 add .를 같이할 수 있는 명령어는 git commit -am "commit message"이다.![](https://velog.velcdn.com/images/eungbi/post/7a9aa516-cb5c-45c3-9ab4-d5b0603a6e73/image.png)

### 4) git push / git push origin master

<br> 로컬 저장소의 변경사항을 원격 저장소(GitHub)에 업로드한다.

- **git push만 사용하는 경우:**
  Git에 이미 원격 저장소와 현재 브랜치에 대한 기본값이 설정되어 있다면, git push 명령어만 작성해도된다. 이는 Git이 설정 파일에서 현재 브랜치와 연결된 원격 브랜치를 찾아 해당 브랜치로 변경사항을 업로드한다.![](https://velog.velcdn.com/images/eungbi/post/182506e8-8927-43df-b3bf-391a1073835f/image.png)
- **git push origin master 사용하는 경우:**
  여러 원격 저장소가 있거나, 혹은 여러 브랜치를 사용하는 복잡한 프로젝트에서 유용하다.
  또한, 로컬 저장소의 브랜치와 원격 저장소의 브랜치가 자동으로 연결되지 않았거나, 기본 설정을 변경하고 싶을 때 이 명령어를 사용한다.<br>
  ![](https://velog.velcdn.com/images/eungbi/post/1510a658-4b4d-44ae-8b70-b80ea5268b40/image.png)<br>결론적으로, git push만 사용하는 것은 일반적으로 더 간단하고 편리하지만, 원격 저장소나 브랜치가 여러 개 있거나, 특정한 설정을 사용하고 싶을 때는 git push origin master와 같은 구체적인 명령어를 사용하는 것이 좋다.

### 5) git pull

<br> 원격 저장소의 최신 변경사항을 로컬 저장소로 가져온다.
![](https://velog.velcdn.com/images/eungbi/post/30792c6a-6bc9-404f-9327-9715910ebdcc/image.png)

### 6) git branch

<br> 현재 있는 브랜치를 확인하거나 새로운 브랜치를 생성한다.![](https://velog.velcdn.com/images/eungbi/post/1c89513b-4bb8-4513-ad53-72b7c3255f4d/image.png)

- git branch [브랜치명]: 새 브랜치 생성
- git branch -d [브랜치명]: 브랜치 삭제
- git branch -D [브랜치명]: 강제 브랜치 삭제
- git branch -a: 로컬과 원격 브랜치 모두 보기

### 7) git checkout [브랜치명]

<br> 다른 브랜치로 전환한다.![](https://velog.velcdn.com/images/eungbi/post/cb33d510-c3c8-4749-98e6-ea33bed6800d/image.png)

### 8) git merge [브랜치명]

<br> 다른 브랜치의 변경사항을 현재 브랜치와 합친다.![](https://velog.velcdn.com/images/eungbi/post/8ff4bd6b-69d3-474a-b914-523cc813d9d2/image.png)
