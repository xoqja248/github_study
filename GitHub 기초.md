# GitHub 기초



## 1. Git 초기 설정 

1. 커밋 기록을 확인하기 위한 이름과 이메일을 설정한다.

   ```bash
   $ git config --global user.name "UserName"
    
    $ git config --global user.email "EmailAdress"
   ```

   


2. 작성자가 올바르게 설정되었는지 확인

   ```bash
   $ git config --global -1    
           
          or    
          
   $ git config --global --list
   ```

   

## 2. Git 기본 명령어

1.  ``git init``
   - 현재 작업중인 디렉토리를 Git으로 관리한다는 명령어
   - 설정 완료시 디렉토리 이름 옆에 (master) 표기 됨
2.  ``git status``
   - Working Directory와  Staging Area에 있는 파일의 현재 상태를 보여줌
 	3. ``git add``
     - Working Directory에 있는 파일을 Staging Area로 올리는 명령어
4. ``git commit``
   - Staging Area에 올라온 파일을 하나의 버전(커밋)으로 저장하는 명령어
5.  ``git log``

   - 커밋의 내역을 조회한다. 
   - 옵션
     - `--oneline` : 한 줄로 요약해서 보여줌
     - `--graph` : branch와 merge 내역을 그래프로 보여줌
     - `--all` : 현재 branch를 포함한 모든 내역을 보여줌
     - `--reverse` : 커밋 내역을 반대 순서로 보여줌
     - `--p` : 파일의 변경 내용도 보여줌
     - `--숫자` : 원하는 갯수의 내역을 보여줌




## 3 .GitHub 사용하기 (Remote Repositary)

### 로컬 저장소와 원격 저장소의 연결

1. `git remote add <이름> <주소>`

​		: 원격 저장소를 등록

2. `git remote -v`

   : 원격 저장소 조회

3. `git remote rm <이름>`

   : 로컬과 원격 저장소의 연결 끊기 (원격 저장소를 삭제하는 것은 아님)

### 원격 저장소에 업로드 

1. 커밋 생성

2. `git push <저장소 이름> <branch 이름>`

   : 로컬 장소의 커밋을 원격 저장소에 업로드

   옵션 `-u`를 주면 두번째 커밋부터는 <저장소 이름> <branch 이름> 생략가능

   

### 업로드 예외 처리

- .gitignore

  특정 파일 혹은 폴더에 대해 Git이 버전관리를 하지 못하도록 지정하는 것 (ex > 개인정보, API KEY 등)

- .gitignore 작성을 도와주는 사이트, 개발환경에 따라 자동으로 발생되는 파일들을 가려줌.

  - https://www.toptal.com/developers/gitignore
