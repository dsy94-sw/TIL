## Git 기초

`Git` 이란 분산형버전관리시스템(DVCS-Distributed Version Control System)이라 한다.

# 기초 명령어

![lifecycle](Git 기초.assets/lifecycle-1609231983320.png)

### 1. 저장소 설정

`$ git init` 해당 Directory에 저장소를 설정

이후 설정된 하위폴더 모두 Tracking이 가능

![image-20201229162131440](Git 기초.assets/image-20201229162131440.png)

- (Master)의 유무를 반드시 확인할 것

  ---

  

### 2. add

`touch xx.txt`로 텍스트 파일 생성

`git add xx.txt`명령어를 통해 `working directory`에서  `stage area` 로 이동

```git
$ touch xx.txt
$ git add xx.txt  
```



모든 파일 선택 시  `git add .`  (리숙스에서 `.` 은 현재 Directory를 의미)

```git
$ git add .
```



`git restore --staged <file>` 을 통해 `unstage`(`stage area`에서 `working directory`로) 가능

```git
$ git restore --staged xx.txt
```

---



### 3. commit

`git commit` 은 `stage`에 있는 file의 현재 소스코드 상태를 기록

```git
$ git commit -m "message"
```

---

### 4. status

현재 git의 상태를 확인

```git
$ git status
```

---



### 5. 기타 명령어

- `mkdir <file>` : file이름의 Directory 생성
- `touch <file.확장명>` : file이름의 파일 생성
- `cd (~/./..)` : (home/뒤로가기/위로가기) Directory 이동
- `ls (-a)` : (`-a`포함 시 숨겨진 파일 포함)현재 Directory의 파일 list 확인 
- CLI 문서 편집기 vim
  - `i` : insert 모드
  - `esc` : 명령모드 진입
    - `w` : CLI 문서 저장
    - `q` : CLI 문서 종료
    - `wq` : CLI 문서 저장 후 종료
    - `q!` : CLI 문서 강제 종료

---

