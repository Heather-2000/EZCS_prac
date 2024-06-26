# 환경
python=3.11

# KT에이블스쿨 5기 충남/충북 21조 

## 기본 커맨드 모음
- git init : 현재 디렉토리를 Git이 관리하는 프로젝트 디렉토리(=working directory)로 - 설정하고 그 안에 레포지토리(.git 디렉토리) 생성
- git config user.name 'codeit' : 현재 사용자의 아이디를 'codeit'으로 설정(커밋할 - 때 필요한 정보)
- git config user.email 'teacher@codeit.kr' : 현재 사용자의 이메일 주소를 - 'teacher@codeit.kr'로 설정(커밋할 때 필요한 정보)
- git add [파일 이름] : 수정사항이 있는 특정 파일을 staging area에 올리기
- git add [디렉토리명] : 해당 디렉토리 내에서 수정사항이 있는 모든 파일들을 staging - area에 올리기
- git add . : working directory 내의 수정사항이 있는 모든 파일들을 staging area에 - 올리기
- git reset [파일 이름] : staging area에 올렸던 파일 다시 내리기
- git status : Git이 현재 인식하고 있는 프로젝트 관련 내용들 출력(문제 상황이 - 발생했을 때 현재 상태를 파악하기 위해 활용하면 좋음)
- git commit -m "커밋 메시지" : 현재 staging area에 있는 것들 커밋으로 남기기
- git help [커맨드 이름] : 사용법이 궁금한 Git 커맨드의 공식 메뉴얼 내용 출력
- 
- 
- git remote add origin 주소
- git branch -M main
- git push -u origin main : 로컬 레포지토리의 내용을 처음으로 리모트 레포지토리에 - 올릴 때 사용합니다.(-u origin master가 무슨 뜻인지는 'Git에서 브랜치 사용하기' - 챕터에서 배울 거니까 걱정마세요!)
- git push : 로컬 레포지토리의 내용을 리모트 레포지토리에 보내기
- git pull : 리모트 레포지토리의 내용을 로컬 레포지토리로 가져오기
- git clone [프로젝트의 GitHub 상 주소] : GitHub에 있는 프로젝트를 내 컴퓨터로 - 가져오기git log : 커밋 히스토리를 출력
- git log --pretty=oneline : --pretty 옵션을 사용하면 커밋 히스토리를 다양한 - 방식으로 출력할 수 있습니다. --pretty 옵션에 oneline이라는 값을 주면 커밋 하나당 한 - 줄씩 출력해줍니다. --pretty 옵션에 대해 더 자세히 알고싶으면 이 링크를 참고하세요.
- git show [커밋 아이디] : 특정 커밋에서 어떤 변경사항이 있었는지 확인
- git commit --amend : 최신 커밋을 다시 수정해서 새로운 커밋으로 만듦
- git config alias.[별명] [커맨드] : 길이가 긴 커맨드에 별명을 붙여서 이후로 - 별명으로 해당 커맨드를 실행할 수 있도록 설정
- git diff [커밋 A의 아이디] [커밋 B의 아이디] : 두 커밋 간의 차이 비교
- git reset [옵션] [커밋 아이디] : 옵션에 따라 하는 작업이 달라짐(옵션을 생략하면 - --mixed 옵션이 적용됨)(2) staging area도 특정 커밋처럼 리셋(--mixed는 여기까지 - 수행)그리고 이때 커밋 아이디 대신 HEAD의 위치를 기준으로 한 표기법(예 : HEAD^, - HEAD~3)을 사용해도 됨
- (3) working directory도 특정 커밋처럼 리셋(--hard는 여기까지 수행)
- (1) HEAD가 특정 커밋을 가리키도록 이동시킴(--soft는 여기까지 수행)
- git tag [태그 이름] [커밋 아이디] : 특정 커밋에 태그를 붙임
- git branch [새 브랜치 이름]: 새로운 브랜치를 생성
- git checkout -b [새 브랜치 이름]: 새로운 브랜치를 생성하고 그 브랜치로 바로 이동
- git branch -d [기존 브랜치 이름]: 브랜치 삭제
- git checkout [기존 브랜치 이름]: 그 브랜치로 이동
- git merge [기존 브랜치 이름]: 현재 브랜치에 다른 브랜치를 머지
- git merge --abort: 머지를 하다가 conflict가 발생했을 때, 일단은 머지 작업을 - 취소하고 이전 상태로 돌아감- git show [커밋 아이디] : 특정 커밋에서 어떤 변경사항이 있었는지 확인
- git commit --amend : 최신 커밋을 다시 수정해서 새로운 커밋으로 만듦
- git config alias.[별명] [커맨드] : 길이가 긴 커맨드에 별명을 붙여서 이후로 - 별명으로 해당 커맨드를 실행할 수 있도록 설정
- git diff [커밋 A의 아이디] [커밋 B의 아이디] : 두 커밋 간의 차이 비교
- git reset [옵션] [커밋 아이디] : 옵션에 따라 하는 작업이 달라짐(옵션을 생략하면 - --mixed 옵션이 적용됨)(2) staging area도 특정 커밋처럼 리셋(--mixed는 여기까지 - 수행)그리고 이때 커밋 아이디 대신 HEAD의 위치를 기준으로 한 표기법(예 : HEAD^, - HEAD~3)을 사용해도 됨
- (3) working directory도 특정 커밋처럼 리셋(--hard는 여기까지 수행)
- (1) HEAD가 특정 커밋을 가리키도록 이동시킴(--soft는 여기까지 수행)
- git tag [태그 이름] [커밋 아이디] : 특정 커밋에 태그를 붙임
- 
- 
- 
- 
- 
- git branch [새 브랜치 이름]: 새로운 브랜치를 생성
- git checkout -b [새 브랜치 이름]: 새로운 브랜치를 생성하고 그 브랜치로 바로 이동
- git branch -d [기존 브랜치 이름]: 브랜치 삭제
- git checkout [기존 브랜치 이름]: 그 브랜치로 이동
- git merge [기존 브랜치 이름]: 현재 브랜치에 다른 브랜치를 머지
- git merge --abort: 머지를 하다가 conflict가 발생했을 때, 일단은 머지 작업을 - 취소하고 이전 상태로 돌아감
