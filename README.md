# Git & GitHub 튜토리얼
이 튜토리얼은 Git의 기본적인 사용 방법과 GitHub을 통한 협업 방법을 소개합니다. Git과 GitHub은 소프트웨어 개발 과정에서 코드의 버전 관리와 팀워크를 강화하는 데 필수적인 도구입니다.
<br><br>

## Git

Git은 분산 버전 관리 시스템으로, 프로젝트의 소스 코드 관리에 널리 사용됩니다.
<br><br>

### 1. Git 설치하기

- [Git 공식 웹사이트](https://git-scm.com)에서 운영 체제에 맞는 Git 버전을 다운로드하고 설치합니다.


### 2. 사용자 설정하기

처음 Git을 사용하는 경우, 사용자 이름과 이메일 주소를 설정해야 합니다. 이 정보는 커밋할 때 마다 사용됩니다.

- **사용자 이름 설정하기**
  ```bash
  git config --global user.name "jjangmo91"
- **이메일 주소 설정하기**
  ```bash
  git config --global user.email "qkqhjjangmo@example.com"
  ```

### 3. 새로운 저장소 만들기

새 디렉토리에서 시작하거나 기존 디렉토리에서 Git 저장소를 초기화할 수 있습니다.
  ```bash
   git init
  ```

### 4. 파일 추가 및 커밋하기

프로젝트에 파일을 추가하거나 변경한 후, 이러한 변경 사항을 저장소에 커밋해야 합니다.
  ```bash
   git add .
   git commit -m "초기 프로젝트 설정"
  ```

### 5. 변경 사항 확인하기
작업한 내용과 저장소 상태를 확인하려면 다음 명령어를 사용합니다.
```bash
   git status
   git log
  ```
<br><br>

## GitHub
GitHub는 Git의 클라우드 기반 호스팅 서비스로, 프로젝트를 공유하고 다른 사람들과 협업하는 데 이상적입니다.
<br><br>

### 1. GitHub에 Repository 만들기
GitHub에서 New Repository를 만듭니다. 이후 생성된 Repository URL을 복사합니다.

### 2. 로컬 저장소와 GitHub Repository 연결하기
로컬 Git 저장소에서 다음 명령어를 사용하여 GitHub Repository를 원격 저장소로 추가합니다.
```bash
   git remote add origin Repository_URL
  ```

### 3. 변경 사항을 GitHub에 푸시하기
로컬 저장소의 변경 사항을 GitHub에 푸시하여 공유합니다.
```bash
   git push -u origin master
  ```

### 4. 변경 사항 가져오기 및 병합하기
다른 사람의 변경 사항을 로컬 저장소로 가져오고 싶을 때는 다음 명령어를 사용합니다.
```bash
   git pull origin master
  ```

### 5. 협업
프로젝트에 기여하고 싶다면, 해당 프로젝트를 fork하고, 변경사항을 commit한 다음, pull request를 생성하여 기여할 수 있습니다.
<br><br>

## 마크다운 사용법
마크다운은 텍스트 기반의 마크업 언어로, 간단한 문법으로 다양한 문서를 꾸밀 수 있습니다. 이 섹션에서는 README 파일 작성에 유용한 마크다운 문법을 소개합니다.


소스코드 블록은 다음과 같이 작성할 수 있습니다.
```c
#include <stdio.h>

int main(void){
  printf("Hello World!");
  return 0;
}
```


링크는 다음과 같이 작성할 수 있습니다.

[블로그 주소](http://https://blog.naver.com/jjangmo91)


순서 없는 목록은 다음과 같이 작성할 수 있습니다.

* 깃 튜토리얼
  * 깃 Clone
  * 깃 pull
  * 깃 commit
     * 깃 commit 1)
     * 깃 commit 2)


인용 구문은 다음과 같이 작성할 수 있습니다.

> '공부합시다' - 성정모 -


테이블은 다음과 같이 작성할 수 있습니다.

 이름|영어|정보|수학
 ---|---|---|---|
 성정모|0점|50점|100점|
 홍길동|84점|97점|42점|
 이순신|100점|100점|100점|

 강조는 다음과 같이 할 수 있습니다.

 **치킨** 먹다가 ~~두드리기~~ 났어요. ㅠ_ㅠ
