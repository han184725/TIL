## cmd, PowerShell

- CLI/GUI
  - CLI: commad line interface
  - GUI: graphical user interface
- Unix/Linux 명령어 git에서 사용0



# 간단한 Unix/Linux 명령어

- 현재 위치의 폴더 파일 목록보기 ls
- 현재 위치 이동하기 cd<path>
- 상위 폴더로 이동 cd ..
- 폴더 생성하기 mkdir<name>
- 파일 생성하기 touch<name>
- 삭제사기 rm<name>, rm-r<name>



# git

- ~ 홈 디렉토리
- `touch name.txt` 파일 생성
- `rm name.txt` 파일 삭제
- `rm -r name` 폴더 삭제
- README.md 프로젝트 설명서 파일
- Repository: 특정 디렉토리를 버전 관리하는 저장소
- `git init` 로컬 저장소 생성
- 특정 버전으로 남긴다 = "커밋(commit)"한다
  - working directory, staging area, repository 바탕 동작
  - working directory: 내가 작업하고 있는 실제 디렉토리(untracked)(-> `git add` -> modified)
  - staging area: 커밋으로 남기고 싶은, 특정 버전으로 관리하고 싶은 파일이 있는 곳(`git add`-> tracked)
  - repository: 커밋들이 저장되는 곳(.git directory)(`git commit` -> committed)
  - `-m ""` 메시지 옵션
- `git status` 관리되고 있는 파일들의 상태
- `git add.` 추적되지 않은 모든 파일과 추적 하고 있는 파일 중 수정된 파일을 모두 staging area에 올림
- `cd ..` 상위 디렉토리로 이동
- `git commit -m "commit_message"`
- `git config user.name "user_name"`
- `git config user.email "user_email"`
- repository 내부에서 repository 만들지 X
- `git diff a b` 앞의 커밋을 기준으로 뒤의 커밋을 비교
- `clone` 처음에 가져오기
- `git push`
- `git pull`
- `git remote add origin url`
- `git push -u origin master`

***

## git 이름, 이메일 변경

- `git config user.name ""`
- `git config user.email ""`
- `git config --unset user.name` 
- `git config --unset user.email`
- `git config --unset --global user.name` 
- `git config --unset --global user.email`
- `git config --global user.name ""`
- `git config --global user.email ""`

