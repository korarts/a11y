# Git 설치
[https://git-scm.com/book/ko/v2/시작하기-Git-설치](https://git-scm.com/book/ko/v2/시작하기-Git-설치)
[git-scm 다운로드](https://git-scm.com/download)
[git Document Book](https://git-scm.com/book/ko/v2)




# Git CLI 명령어
---
* d:\html 폴더 내에 myhome 폴더를 생성함. d:\html\myhome이 로컬 홈페이지 주소
* git-scm 설치 
* 검색 프로그램(window키) 창에서 bash 입력 
* git bash 프로그램을 찾으면 Enter 키로 실행
* cd d:\html 입력 후 실행 (html 폴더 내로 진입)


## 1. config 설정
* 현재 설정정보 조회
	```
	$git config --global --list  
	$git config --list
	```

* <b style="color:crimson">(필수) 사용자명 등록 / 변경</b>
	```
	$git config --global user.name "사용자 아이디"
	```

* <b style="color:crimson">(필수) 이메일 주소 등록 / 변경 </b>
	```
	$git config --global user.email "사용자 이메일주소"
	```

* <b style="color:crimson">(필수) 프로젝트 하나에서만 사용자명 등록 / 변경</b>
	```
	$git config --local user.name "사용자명"
	```

* <b style="color:crimson">(필수) 프로젝트 하나에서만 이메일 주소 등록 / 변경</b>
	```
	$git config --local user.email "이메일주소"
	```

* 사용자명 삭제
	```
	$git config --unset user.name "사용자명"
	```

* 이메일 주소 삭제
	```
	$git config --unset user.email  "이메일주소"
	```


## 2. git 상태
* 현재 git 버전 확인
	```
	$git --version  
	```

* 파일 상태 확인
	```
	$git status  
	```

* 내 컴퓨터 로컬폴더에 서버 저장소 주소 알려주기
	```
	$git remote 
	```

* 마지막 commit 된 내역 조회 명령어
	```
	$git log 
	```

---
## 3. init or clone
* 기존 프로젝트의 디렉토리에 git 저장소로 만들기(.git이라는 하위 디렉토리 생성)
	```
	$git init 
	```

* 명령으로 저장소를 복제
	```
	$git clone git://git사이트에서 제공하는 저장소.git 
	```

---
## 4. 로컬저장소 저장
저장소에 파일 추가하고 커밋함 / 커밋으로 만들길 원하는 파일만 선택
	```
	$git add 파일명.html 
	```

* workign directory 전체를 의미
	```
	$git add .
	```

* 스테이시 파일을 커밋
	```
	$git commit -m "커밋 메세지를 전달하면 주석처럼 메세지 저장됨"
	```

* 스테이시와 커밋을 동시에 (단, 한번도 add되지 않은 파일은 안됨)
	```
	$git commit -am "commit Comment"
	```

---
## 5. remote (원격저장소)

* 현재 연결된 저장소 확인
	```
	$git remote -v
	```

* 새 리모트 저장소 추가
	```
	$git remote add [단축이름\] [url]
	```

* 원격 저장소와의 연결 제거
	```
	$git remote remove origin
	```

---
## 6. remote push
push는 마지막으로 커밋한 사항을 git repository 에 올리겠다는 뜻
* 원격저장소로 push하기 전에 내용이 충돌나지 않도록 pull로 git pull로 먼저 수정내용 확인
	```
	$git pull
	```

* 원격저장소 origin리모트에 로컬에 commit된 것을 push
(origin과 master는 각 리모트 저장소와 브랜치 의미)
	```
	$git push - origin master
	```

---
## 7. branch

* 브랜치 조회
	```
	$git branch 
	```

* name 브랜치로 이동
	```
	$git checkout name 
	```

* 브랜치 작성과 체크아웃을 한번에 실행
	```
	$git checkout -b <branch> 
	```

* 현재 시점에서 name브랜치 생성
	```
	$git branch name 
	```

* $git push origin `<branch name>`
	```
	$git checkout master 
	```

---
### 7-1. git (리모트 브랜치 번외)
존재하는 모든 리모트 브랜치의 정보를 조회
* 현재 존재하는 브랜치 정보가 모두 출력
	```
	$git branch -a 
	```

* remote에 존재하는 브런치 확인
	```
	$git branch --remote 
	```

* 모든 리모트 정보를 업데이트, fetch를 수행
	```
	$git remote update 
	```

* 현재 자신의 로컬에 있는 리모트 브랜치 정보를 최신으로 업데이트. 새로 추가되었거나 삭제된 리모트 브랜치의 정보들을 최신으로 업데이트할 수 있다. 아래의 커맨드와 동작은 같으나 리모트를 선택하여 반영, 업데이트 할 수 있음.
	```
	$git remote prune origin 
	```
* 현재 자신의 로컬에 있는 리모트 브랜치 정보를 최신으로 업데이트
	```
	$git fetch --prune 
	```

---
## 8. log

* commit해둔 기록을 조회 (checkout위치에서 보여줌)
	```
	$git log
	```

* 각 커밋을 한 줄로 표시
	```
	$git log --pretty=oneline
	```

* 현재 위치한 저장소가아닌 전체 저장소를 확인
	```
	$git log --branches
	```

* master와 branch의 표시로 최신 커밋을 보여줌(HEAD 표시로 현재 Checkout된 branch를 보여줌)
	```
	$git log --branches --decorate
	```

* 빨간줄로 흐름을 간단하게 보여줌
	```
	$git log --branches --decorate --graph
	```

---
## 9. merge

* master로 돌아옴 또는 브랜치
	```
	$git checkout master
	```

* 현재 위치한 저장소가 아닌 전체 저장소 확인
	```
	$git merge 브랜치
	```

* merge된 부분 확인
	```
	$git log --branches --grahp --oneline
	```

* merge가 된 branch는 삭제
	```
	$git branch -d 브랜치
	```


* merge 취소
(ORIG_HEAD라고 하는 것은 이전에 작업한 곳의 HEAD 즉, pull이나 merge를 하는 경우에 ORIG_HEAD를 남기게 되는데, pull을 잘못 받거나 merge를 잘못하게 되면 이것을 이용)
	```
	$git reset --merge ORIG_HEAD
	```
* merge 취소 병합(merge) 시에 충돌(conflict) 등의 문제로 병합이 제대로 이루어지지 않을 경우, 병합 이전의 상태로 돌아간다
	```
		$git merge --abort
	```

---
## 10. reset (취소, 수정)

* git add 취소
	```
	$git reset
	```

* 최종 커밋 취소. 그러나 변경된 파일은 남아있다.
	```
	$git reset HEAD^
	```

* 최종 커밋 취소하고 파일 까지 복구한다.
	```
	$git reset --hard HEAD^
	```

* 마지막 n개의 커밋을 취소, 그러나 변경된 파일은 남아 있다.( n : 숫자 )
	```
	$git reset HEAD~n
	```

* 마지막 n개의 커밋을 취소. 파일 또한 복구.
	```
	$git reset --hard HEAD~n
	```


* 스테이징을 언스테이징으로 변경, ref
	```
	$git reset HEAD *
	```

*  git commit --amend 명령어를 입력하면  마지막 커밋메세지 수정(ref)
	```
	$git add 
	```

* 마지막 커밋메세지 수정(ref)
	```
	$git commit --amend -m "33"
	```

* local 브랜치 삭제$git push origin :삭제된 브랜치명 :  remote 브랜치 삭제
	```
	$git branch -d 삭제할 브랜치명
	```
* ref 브랜치 삭제
	```
	$git fetch --prune 
	```

### 11. remote branch
- 삭제할 브런치외에 다른 브런치로 checkout
어떤 브런치가 있는지 확인 
	```
	$git remote show origin
	```

* 삭제할 브랜치명 : local 브랜치 삭제 1번
	```
	$git branch -D 
	```
* 2번
	```
	$git push origin –delete  
	$git push origin :branch_name 
	ex) $git push origin :shopping_cart : 원격에 있는 브랜치를 삭제.
	```

* $git remote prune은 리모트 브랜치의 더 이상 유효하지 않은 참조를 깨끗이 지우는 명령어 
	```
	$git remote prune 
	$git remote prune origin : remote 브랜치 clean up 하기 
	$git remote update –prune
	```

#### 11_1. 축약버전 
	```
	$git branch –delete –remotes
	$git branch -dr : 위 명령어의 축약버전 
	$git fetch --prune : 유효하지 않은 tracking 브랜치들을 일괄 삭제한다 
	$git fetch -p # 축약 버전
	```

## 12. git stash
* marke git stash 
	```
	$git stash : 아직 마무리하지 않은 작업을 스택에 잠시 저장할 수 있도록 하는 명령어
	$git stash save 작업명 : #stash에 작업명의 이름으로 임시 저장 
	$git stash list : 스택에 있는 stash 목록 확인
	```

* git stash 적용 
	```
	$git stash apply : 가장 최근의 stash 적용 
	$git stash apply [stash 이름] : [stash 이름]에 해당하는 stash 적용 
	$git stash apply –index : [stash 이름]에 해당하는 stash 적용
	```

## [index 유무의 차이]

	```
	git stash apply & git stahs apply –index
	```
수정했던 파일들을 복원할 때 반드시 stash했을 때와 같은 브랜치일 필요는 없다. 
만약 다른 작업 중이던 브랜치에 이전의 작업들을 추가했을 때 충돌이 있으면 알려준다.
index 옵션을 주어 staged 상태까지 적용. 원래 작업하던 상태로 돌아올 수 있다.

* git stash제거 
	```
	$git stash pop : apply + drop의 형태로, 현재브런치에 저장내용을 복구, status 결과와 함께 스텍에도 목록 제거 
	(마지막으로 저장된 stash작업을 불러오고 리스트에서 삭제)
	```
* git stash 되돌리기 
	```
	$git stash show -p | git apply -R 
	: 가장 최근의 stash를 사용하여 패치를 만들고 거꾸로 적용 
	$git stash show -p [stash 이름] | git apply -R
	```

## 13. git 충돌

	```
	$git push -f : 아직 마무리하지 않은 작업을 스택에 잠시 저장할 수 있도록 하는 명령어 
	$git push –force 작업명 : #stash에 작업명의 이름으로 임시저장 
	$git push origin +<branch_name> : 스택에 있는 stash 목록 확인
	```

* git rebase - merge를 사용하는 것보다 rebase를 사용하는 것이 로그를 관리할 때 훨씬 효과적입니다.
git merge는 header와 branch를 merge시키고, rebase는 commit을 재정렬한다.
rebase를 하게 되면 커밋도 새로 쓰고 정렬도 새로 하기 때문에 기존 커밋트리가 완전히 달라진다.

---
## 14. git reset
작업을 진행하다가 실수로 중요한 파일을 삭제했거나 제대로 병합이 안됐을 경우, 잘 작동이 되던 이전 버전으로 돌아가야 합니다.
이것이 바로 버전 관리를 하는 이유이며, 이 때 사용하는 명령어가 git reset과 git revert라는 명령어입니다.

	```
	$  git reset  HEAD^
	$  git reset [commit ID]
	```

* git reset 취소
reset을 한 상태에서 다시 최근 소스로 돌아오기 위해서 사용
	```
	$ git reflog : 이전까지 작업들 reflog로 확인 몇번째 HEAD로 이동할지 확인
	$ git reset --hard HEAD@{1} : HEAD@{1} 로 이동
	$ git push -f origin [브랜치명] : 돌아간 시장을 강제로 push
	```

* git reset 되돌리기
git reset으로 실수로 저장없는 전버전으로 돌려놨을 때
	```
	$  git reset --hard HEAD^
	$  git reflog
	$  git reset HEAD@{1}
	```

### HEAD의 여러 표현 방법
```
  HEAD^[n] : n번째 부모 버전  (the parent of HEAD), 생략시 1
  HEAD~[n] : n번째 부모의 부모. (the first parent of the first parent or the grandparent)
  HEAD~ 와 HEAD^ 는 같은 대상이지만 특정숫자들을 입력하면 대상이 달라진다. (HEAD^4 와 HEAD~4 는 다르다.) 하지만 다음 예제는 같은 커밋개체을 가르킨다.
  HEAD^^^ == HEAD~3    (HEAD^^^ 가 첫번째부모의 첫번째부모의 첫번째부모 노드를 뜻하므로 같은 값을 가르킨다.)
```

### reset 옵션
```
  git reset --hard 커밋ID : 모든 내용을 지우고 되돌아감(초기화)
  git reset --soft 커밋ID : 커밋은 되돌렸지만 코드의 내용은 변경되지 않음
  git reset --mixed 커밋ID : 옵션을 설정하지 않았을때 기본값 
  (커밋 되돌렸고, 변경된 내용이 남아있어서 다시 추가할수 있음 )
```

### 단골에러
```
  To https://github.com/hahwul/a2sv.git
  ! [rejected]        master * master (non-fast-forward)
  error: failed to push some refs to 'https://github.com/dabin-lee/ddbb'
  hint: Updates were rejected because the tip of your current branch is behind
  hint: its remote counterpart. Merge the remote changes (e.g. 'git pull')
  hint: before pushing again.
  hint: See the 'Note about fast-forwards' in 'git push --help' for details.
``` 
* 실제 에러가 발생하는 부분을 고칠수도 있지만 임시 방편으로 “+” 를 이용하여 해결이 가능합니다.
* 아래와 같이 강제로 push 를 진행하게 되면 에러 상관없이 강제로 Push 하게 되어 이슈를 넘어갈 수 있습니다. [물론 임시 방편입니다.]
	* 기존명령: `git push -u origin master`
	* 강제명령: `git push -u origin +master`

---
## 15. git ignore
* 버전관리 중 불필요한 파일
* ex) 자바 프로젝트에서 컴파일을 하면 .class 파일들이 생성되는데 github와 같은 저장소에 .class 제외하고 .java 파일만 올리고 싶을 경우에 이와 같은 역할을 해주는 것이 .gitignore !gitignore;

| #, 빈라인	| #은 주석을 의미하며, 빈라인은 아무런 영향을 주지 않습니다.|
| -- | -- |
| *.a | 확장자가 .a 인 모든 파일을 무시합니다.
| folder_name/ | 해당 폴더의 모든 파일을 무시합니다.
| folder_name/ *.a | 해당 폴더의 확장자가 .a 인 모든 파일을 무시합니다.
| folder_name/ */.a | 해당 폴더 포함한 하위 모든 폴더에서 확장자가 .a 인 모든 파일을 무시합니다.
| /*.a | 현재 폴더의 확장자가 .a 인 모든파일을 무시합니다.

* git ignore가 반영되지 않을 때
```
  $git rm -r --cached .
  $git add .
  $git commit -m "git ignore add"
  $git push
```

---
## 16. git archive
* 폴더를 압축하고 .git 하위 폴더를 제외시키는 방법
	```
	$ git archive -o 프로젝트.zip HEAD 
	Git에 저장된 프로젝트를 압축하려는 경우 git archive명령을 사용
	$ git archive -o test.zip HEAD $(git diff --name-only HEAD^) 
	최종 커밋 내용 zip 파일로 압축
	```