# GitHub 기초



## 1. Git 초기 설정 

1.   커밋 기록을 확인하기 위한 이름과 이메일을 설정한다.

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

   



