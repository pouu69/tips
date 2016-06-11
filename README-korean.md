<!-- @doxie.inject start toc -->
<!-- Don’t remove or change the comment above – that can break automatic updates. -->
* [매일 만나는 Git 명령어 20가지](#매일-만나는-git-명령어-20가지)
* [유용한 Git 가이드 목록 보기 ](#유용한-git-가이드-목록-보기)
* [원격리파지토리 내용으로 덮어쓰기](#원격리파지토리-내용으로-덮어쓰기)
* [특정 커밋까지의 모든 파일 목록 보기](#특정-커밋까지의-모든-파일-목록-보기)
* [최초 커밋으로 초기화하기 ](#최초-커밋으로-초기화하기)
* [충돌난 파일 목록 모두 보기 ](#충돌난-파일-목록-모두-보기)
* [특정 커밋에서 변경된 파일 목록 보기 ](#특정-커밋에서-변경된-파일-목록-보기)
* [스테이지 되지 않은 최종 커밋 이후에 변경된 내용 보기](#스테이지-되지-않은-최종-커밋-이후에-변경된-내용-보기)
* [스테이지된 변경사항 확인하기](#스테이지된-변경사항-확인하기)
* [모든 변경사항 확인하기 ](#모든-변경사항-확인하기)
* [마스터에 이미 머지된 모든 브랜치 목록 모두 보기 ](#마스터에-이미-머지된-모든-브랜치-목록-모두-보기)
* [이전에 브랜치로 빠르게 이동하기 ](#이전에-브랜치로-빠르게-이동하기)
* [마스터에 머지된 브랜치 삭제하기 ](#마스터에-머지된-브랜치-삭제하기)
* [원격리파지토리와 최종 커밋을 같이 표시하면서 모든 브랜치 목록보기](#원격리파지토리와-최종-커밋을-같이-표시하면서-모든-브랜치-목록보기)
* [원격리파지토리의 브랜치 변경사항 확인하기](#원격리파지토리의-브랜치-변경사항-확인하기)
* [로컬리파지토리의 브랜치 삭제하기 ](#로컬리파지토리의-브랜치-삭제하기)
* [원격리파지토리의 브랜치 삭제하기 ](#원격리파지토리의-브랜치-삭제하기)
* [최종 커밋이후의 로컬리파지토리 파일의 변경된 내용 되돌리기 ](#최종-커밋이후의-로컬리파지토리-파일의-변경된-내용-되돌리기)
* [되돌리기(Revert): 되돌리는 새로운 커밋을 만듬](#되돌리기(revert):-되돌리는-새로운-커밋을-만듬)
* [되돌리기(Reset): 커밋들을 취소, 혼자만 사용하는 브랜치에서만 할 것을 추천함](#되돌리기(reset):-커밋들을-취소,-혼자만-사용하는-브랜치에서만-할-것을-추천함)
* [이전 커밋메시지 수정하기 ](#이전-커밋메시지-수정하기)
* [작성자 수정하기.](#작성자-수정하기.)
* [전역에 작성자를 설정한 이후, 커밋의 작성자 변경하기 ](#전역에-작성자를-설정한-이후,-커밋의-작성자-변경하기)
* [원격리파지토리 주소(URL) 변경하기 ](#원격리파지토리-주소(url)-변경하기)
* [원격 리파지토리 모든 목록 보기](#원격-리파지토리-모든-목록-보기)
* [로컬리파지토리와 원격리파지토리의 모든 브랜치 확인하기 ](#로컬리파지토리와-원격리파지토리의-모든-브랜치-확인하기)
* [원격리파지토리의 모든 브랜치 보기 ](#원격리파지토리의-모든-브랜치-보기)
* [전체 파일 대신에 변경된 파일만 스테이지하기 ](#전체-파일-대신에-변경된-파일만-스테이지하기)
* [Bash에서 자동완성 설정하기](#bash에서-자동완성-설정하기)
* [최근 2주간 변경사항 확인하기 ](#최근-2주간-변경사항-확인하기)
* [마스터에서 분기된 이후의 모든 변경사항 확인하기 ](#마스터에서-분기된-이후의-모든-변경사항-확인하기)
* [체리픽명령(cherry-pick)으로 다른 브랜치의 커밋 가져오기 ](#체리픽명령(cherry-pick)으로-다른-브랜치의-커밋-가져오기)
* [특정 커밋을 포함하는 브랜치 찾기 ](#특정-커밋을-포함하는-브랜치-찾기)
* [Git 명령에 별칭 주기 ](#git-명령에-별칭-주기)
* [형상관리 되는 파일의 변경사항을 커밋하지 않고 저장하기 ](#형상관리-되는-파일의-변경사항을-커밋하지-않고-저장하기)
* [모든 파일의 변경사항을 커밋하지 않고 저장하기 ](#모든-파일의-변경사항을-커밋하지-않고-저장하기)
* [저장된 목록 모두 보기 ](#저장된-목록-모두-보기)
* [저장된 목록에서 목록을 삭제하지 않고 변경사항 적용하기](#저장된-목록에서-목록을-삭제하지-않고-변경사항-적용하기)
* [저장된 목록에서 마지막으로 기록된 내용을 지우고 그때의 변경사항을 적용하기 ](#저장된-목록에서-마지막으로-기록된-내용을-지우고-그때의-변경사항을-적용하기)
* [저장된 내용 모두 지우기 ](#저장된-내용-모두-지우기)
* [저장된 내용으로 부터 파일 하나만 꺼내기 ](#저장된-내용으로-부터-파일-하나만-꺼내기)
* [형상관리 되는 파일 모두 보기 ](#형상관리-되는-파일-모두-보기)
* [형상관리 되지 않는 파일 모두 보기 ](#형상관리-되지-않는-파일-모두-보기)
* [제외 목록에 있는 파일 모두 보기 ](#제외-목록에-있는-파일-모두-보기)
* [리파지토리에서 새로운 작업트리 생성하기 (git 2.5)](#리파지토리에서-새로운-작업트리-생성하기-(git-2.5))
* [최종상태의 새로운 작업트리 생성하기 ](#최종상태의-새로운-작업트리-생성하기)
* [삭제하지 않고 형상관리 대상에서 제외하기 ](#삭제하지-않고-형상관리-대상에서-제외하기)
* [형상괸리 되지 않는 파일을 삭제하기 전에, 모의로 수행해보기 ](#형상괸리-되지-않는-파일을-삭제하기-전에,-모의로-수행해보기)
* [형상관리 되지 않는 파일을 강제로 삭제하기 ](#형상관리-되지-않는-파일을-강제로-삭제하기)
* [형상관리 되지 않는 디렉토리를 강제로 삭제하기 ](#형상관리-되지-않는-디렉토리를-강제로-삭제하기)
* [모든 서브모듈을 업데이트 하기 ](#모든-서브모듈을-업데이트-하기)
* [현재 브랜치에서 마스터로 머지되지 않은 목록 모두 보기 ](#현재-브랜치에서-마스터로-머지되지-않은-목록-모두-보기)
* [브랜치 이름 변경하기 ](#브랜치-이름-변경하기)
* [마스터의 변경사항을 반영하고, 마스터에 머지하기 ](#마스터의-변경사항을-반영하고,-마스터에-머지하기)
* [마스터 브랜치를 압축하기 ](#마스터-브랜치를-압축하기)
* [커밋 메시지는 수정하지 않고 이전 커밋을 수정하기 ](#커밋-메시지는-수정하지-않고-이전-커밋을-수정하기)
* [현재 접근할 수 없는 오브젝트들을 삭제하기 .](#현재-접근할-수-없는-오브젝트들을-삭제하기-.)
* [최초의 커밋 이력을 조회하기 ](#최초의-커밋-이력을-조회하기)
* [Git 로그를 시각화하기](#git-로그를-시각화하기)
* [형상관리 되고 있는 하위폴더를 gh-pages로 배포하기 ](#형상관리-되고-있는-하위폴더를-gh-pages로-배포하기)
* [하위 폴더를 사용하는 프로젝트 리파지토리 추가하기 ](#하위-폴더를-사용하는-프로젝트-리파지토리-추가하기)
* [하위 폴더를 사용하여 연결된 프로젝트를 위해 리파지토리의 최근 변경사항 확인하기 ](#하위-폴더를-사용하여-연결된-프로젝트를-위해-리파지토리의-최근-변경사항-확인하기)
* [파일의 변경 이력을 포함하여 번들 내보내기 ](#파일의-변경-이력을-포함하여-번들-내보내기)
* [번들 읽어오기 ](#번들-읽어오기)
* [현재 브랜치의 이름 확인하기 ](#현재-브랜치의-이름-확인하기)
* [커밋에서 파일 하나 제외하기 (예. Changelog).](#커밋에서-파일-하나-제외하기-(예.-changelog).)
* [리베이스 하기 전에 저장하기 ](#리베이스-하기-전에-저장하기)
* [원격리파지토리의 변경사항을 로컬브랜치로 이동합니다. ](#원격리파지토리의-변경사항을-로컬브랜치로-이동합니다.)
* [현재브랜치에서 가장 최근에 태깅뇐 내용 보여주기 ](#현재브랜치에서-가장-최근에-태깅뇐-내용-보여주기)
* [변경사항 확인하기 .](#변경사항-확인하기-.)
* [형상관리 되는 파일의 변경사항을 변경되지 않은 것으로 표시하기 ](#형상관리-되는-파일의-변경사항을-변경되지-않은-것으로-표시하기)
* [변경되지 않았다고 표시된 내용을 되돌리기.](#변경되지-않았다고-표시된-내용을-되돌리기.)
* [제외된 목록으로부터 필요없는 파일 삭제하기 ](#제외된-목록으로부터-필요없는-파일-삭제하기)
* [삭제된 파일 복구하기 ](#삭제된-파일-복구하기)
* [파일을 특정 커밋으로 되돌리기 ](#파일을-특정-커밋으로-되돌리기)
* [원격리파지토리의 내용을 받아올때 머지 대신에 리베이스하기 ](#원격리파지토리의-내용을-받아올때-머지-대신에-리베이스하기)
* [Git 설정 모두 보기 ](#git-설정-모두-보기)
* [대소문자 구별하도록 설정하기 ](#대소문자-구별하도록-설정하기)
* [오탈자 자동 수정하기 ](#오탈자-자동-수정하기)
* [특정 릴리즈의 변경사항이었는지 확인하기 ](#특정-릴리즈의-변경사항이었는지-확인하기)
* [모의 수행. ( 모든 명령어가 dry-run 옵션을 지원함. ))](#모의-수행.-(-모든-명령어가-dry-run-옵션을-지원함.-)))
* [이전 커밋을 수정했다고 혀냊 커밋에 표시하기 ](#이전-커밋을-수정했다고-혀냊-커밋에-표시하기)
* [커밋과 수정된 커밋을 하나로 합치기 ](#커밋과-수정된-커밋을-하나로-합치기)
* [커밋하는 동안 스테이지에 넣는 행동 생략하기 ](#커밋하는-동안-스테이지에-넣는-행동-생략하기)
* [제외된 파일 목록 보기 ](#제외된-파일-목록-보기)
* [제외된 파일들의 현재상태 확인하기 .](#제외된-파일들의-현재상태-확인하기-.)
* [브랜치1의 커밋을 브랜치2에 커밋하기 ](#브랜치1의-커밋을-브랜치2에-커밋하기)
* [현재의 이전의 충돌 해법을 기록하고ㅓ 재사용하도록 설정하기 ](#현재의-이전의-충돌-해법을-기록하고ㅓ-재사용하도록-설정하기)
* [충돌이 발생한 모든 파일을 에디터에서 열기 ](#충돌이-발생한-모든-파일을-에디터에서-열기)
* [디스크를 소비하고있는 압축되지 않은 오브젝트의 갯수 세기 ](#디스크를-소비하고있는-압축되지-않은-오브젝트의-갯수-세기)
* [오브젝트 데이터페이스에서 접근할 수 없는 모든 오브젝트 제외힉 .](#오브젝트-데이터페이스에서-접근할-수-없는-모든-오브젝트-제외힉-.)
* [작업중인 리파지토리를 바로 웹에서 확인하기 ](#작업중인-리파지토리를-바로-웹에서-확인하기)
* [커밋 로그에서 GPG 서명 확인하기 ](#커밋-로그에서-gpg-서명-확인하기)
* [전역 설정 삭제하기 ](#전역-설정-삭제하기)
* [파일 내용만 담고 이력을 가지지 않는 새로운 브랜치 생성하기 ](#파일-내용만-담고-이력을-가지지-않는-새로운-브랜치-생성하기)
* [최종 커밋과 스테이지된 파일의 변경사항 확인하기 ](#최종-커밋과-스테이지된-파일의-변경사항-확인하기)
* [다른 브랜치의 파일 내용 확인하기 .](#다른-브랜치의-파일-내용-확인하기-.)
* [루트와 머지된 커밋 목록만 확인하기](#루트와-머지된-커밋-목록만-확인하기)
* [이전의 두 커밋을 하나로 합치기 ](#이전의-두-커밋을-하나로-합치기)
* [현재 작업중인 브랜치 목록 보기 ](#현재-작업중인-브랜치-목록-보기)

<!-- Don’t remove or change the comment below – that can break automatic updates. More info at <http://npm.im/doxie.inject>. -->
<!-- @doxie.inject end toc -->
<!-- @doxie.inject start -->
<!-- Don’t remove or change the comment above – that can break automatic updates. -->
## 매일 만나는 Git 명령어 20가지
```sh
git help everyday
```

## 유용한 Git 가이드 목록 보기 
```sh
git help -g
```

## 원격리파지토리 내용으로 덮어쓰기
```sh
git fetch --all && git reset --hard origin/master
```

## 특정 커밋까지의 모든 파일 목록 보기
```sh
git ls-tree --name-only -r <commit-ish>
```

## 최초 커밋으로 초기화하기 
```sh
git update-ref -d HEAD
```

## 충돌난 파일 목록 모두 보기 
```sh
git diff --name-only --diff-filter=U
```

## 특정 커밋에서 변경된 파일 목록 보기 
```sh
git diff-tree --no-commit-id --name-only -r <commit-ish>
```

## 스테이지 되지 않은 최종 커밋 이후에 변경된 내용 보기
```sh
git diff
```

## 스테이지된 변경사항 확인하기
```sh
git diff --cached
```

## 모든 변경사항 확인하기 
```sh
git diff HEAD
```

## 마스터에 이미 머지된 모든 브랜치 목록 모두 보기 
```sh
git checkout master && git branch --merged
```

## 이전에 브랜치로 빠르게 이동하기 
```sh
git checkout -
```

## 마스터에 머지된 브랜치 삭제하기 
```sh
git branch --merged | grep -v '\*' | xargs -n 1 git branch -d
```

## 원격리파지토리와 최종 커밋을 같이 표시하면서 모든 브랜치 목록보기
```sh
git branch -vv
```

## 원격리파지토리의 브랜치 변경사항 확인하기
```sh
git branch -u origin/mybranch
```

## 로컬리파지토리의 브랜치 삭제하기 
```sh
git branch -d <local_branchname>
```

## 원격리파지토리의 브랜치 삭제하기 
```sh
git push origin --delete <remote_branchname>
```


__Alternatives:__
```sh
git push origin :<remote_branchname>
```

## 최종 커밋이후의 로컬리파지토리 파일의 변경된 내용 되돌리기 
```sh
git checkout -- <file_name>
```

## 되돌리기(Revert): 되돌리는 새로운 커밋을 만듬
```sh
git revert <commit-ish>
```

## 되돌리기(Reset): 커밋들을 취소, 혼자만 사용하는 브랜치에서만 할 것을 추천함
```sh
git reset <commit-ish>
```

## 이전 커밋메시지 수정하기 
```sh
git commit -v --amend
```

## 작성자 수정하기.
```sh
git commit --amend --author='Author Name <email@address.com>'
```

## 전역에 작성자를 설정한 이후, 커밋의 작성자 변경하기 
```sh
git commit --amend --reset-author --no-edit
```

## 원격리파지토리 주소(URL) 변경하기 
```sh
git remote set-url origin <URL>
```

## 원격 리파지토리 모든 목록 보기
```sh
git remote
```


__Alternatives:__
```sh
git remote show
```

## 로컬리파지토리와 원격리파지토리의 모든 브랜치 확인하기 
```sh
git branch -a
```

## 원격리파지토리의 모든 브랜치 보기 
```sh
git branch -r
```

## 전체 파일 대신에 변경된 파일만 스테이지하기 
```sh
git add -p
```

## Bash에서 자동완성 설정하기
```sh
curl https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash > ~/.git-completion.bash && echo '[ -f ~/.git-completion.bash ] && . ~/.git-completion.bash' >> ~/.bashrc
```

## 최근 2주간 변경사항 확인하기 
```sh
git whatchanged --since='2 weeks ago'
```

## 마스터에서 분기된 이후의 모든 변경사항 확인하기 
```sh
git log --no-merges --stat --reverse master..
```

## 체리픽명령(cherry-pick)으로 다른 브랜치의 커밋 가져오기 
```sh
git checkout <branch-name> && git cherry-pick <commit-ish>
```

## 특정 커밋을 포함하는 브랜치 찾기 
```sh
git branch -a --contains <commit-ish>
```


__Alternatives:__
```sh
git branch --contains <commit-ish>
```

## Git 명령에 별칭 주기 
```sh
git config --global alias.<handle> <command> 
git config --global alias.st status
```

## 형상관리 되는 파일의 변경사항을 커밋하지 않고 저장하기 
```sh
git stash
```


__Alternatives:__
```sh
git stash save
```

## 모든 파일의 변경사항을 커밋하지 않고 저장하기 
```sh
git stash save -u
```


__Alternatives:__
```sh
git stash save --include-untracked
```

## 저장된 목록 모두 보기 
```sh
git stash list
```

## 저장된 목록에서 목록을 삭제하지 않고 변경사항 적용하기
```sh
git stash apply <stash@{n}>
```

## 저장된 목록에서 마지막으로 기록된 내용을 지우고 그때의 변경사항을 적용하기 
```sh
git stash pop
```


__Alternatives:__
```sh
git stash apply stash@{0} && git stash drop stash@{0}
```

## 저장된 내용 모두 지우기 
```sh
git stash clear
```


__Alternatives:__
```sh
git stash drop <stash@{n}>
```

## 저장된 내용으로 부터 파일 하나만 꺼내기 
```sh
git checkout <stash@{n}> -- <file_path>
```


__Alternatives:__
```sh
git checkout stash@{0} -- <file_path>
```

## 형상관리 되는 파일 모두 보기 
```sh
git ls-files -t
```

## 형상관리 되지 않는 파일 모두 보기 
```sh
git ls-files --others
```

## 제외 목록에 있는 파일 모두 보기 
```sh
git ls-files --others -i --exclude-standard
```

## 리파지토리에서 새로운 작업트리 생성하기 (git 2.5)
```sh
git worktree add -b <branch-name> <path> <start-point>
```

## 최종상태의 새로운 작업트리 생성하기 
```sh
git worktree add --detach <path> HEAD
```

## 삭제하지 않고 형상관리 대상에서 제외하기 
```sh
git rm --cached <file_path>
```


__Alternatives:__
```sh
git rm --cached -r <directory_path>
```

## 형상괸리 되지 않는 파일을 삭제하기 전에, 모의로 수행해보기 
```sh
git clean -n
```

## 형상관리 되지 않는 파일을 강제로 삭제하기 
```sh
git clean -f
```

## 형상관리 되지 않는 디렉토리를 강제로 삭제하기 
```sh
git clean -f -d
```


__Alternatives:__
```sh
git clean -df
```

## 모든 서브모듈을 업데이트 하기 
```sh
git submodule foreach git pull
```

## 현재 브랜치에서 마스터로 머지되지 않은 목록 모두 보기 
```sh
git cherry -v master
```


__Alternatives:__
```sh
git cherry -v master <branch-to-be-merged>
```

## 브랜치 이름 변경하기 
```sh
git branch -m <new-branch-name>
```


__Alternatives:__
```sh
git branch -m [<old-branch-name>] <new-branch-name>
```

## 마스터의 변경사항을 반영하고, 마스터에 머지하기 
```sh
git checkout feature && git rebase @{-1} && git checkout @{-2} && git merge @{-1}
```

## 마스터 브랜치를 압축하기 
```sh
git archive master --format=zip --output=master.zip
```

## 커밋 메시지는 수정하지 않고 이전 커밋을 수정하기 
```sh
git add --all && git commit --amend --no-edit
```

## 현재 접근할 수 없는 오브젝트들을 삭제하기 .
```sh
git fetch -p
```


__Alternatives:__
```sh
git remote prune origin
```

## 최초의 커밋 이력을 조회하기 
```sh
 git rev-list --reverse HEAD | head -1
```

## Git 로그를 시각화하기
```sh
git log --pretty=oneline --graph --decorate --all
```


__Alternatives:__
```sh
gitk --all
```

## 형상관리 되고 있는 하위폴더를 gh-pages로 배포하기 
```sh
git subtree push --prefix subfolder_name origin gh-pages
```

## 하위 폴더를 사용하는 프로젝트 리파지토리 추가하기 
```sh
git subtree add --prefix=<directory_name>/<project_name> --squash git@github.com:<username>/<project_name>.git master
```

## 하위 폴더를 사용하여 연결된 프로젝트를 위해 리파지토리의 최근 변경사항 확인하기 
```sh
git subtree pull --prefix=<directory_name>/<project_name> --squash git@github.com:<username>/<project_name>.git master
```

## 파일의 변경 이력을 포함하여 번들 내보내기 
```sh
git bundle create <file> <branch-name>
```

## 번들 읽어오기 
```sh
git clone repo.bundle <repo-dir> -b <branch-name>
```

## 현재 브랜치의 이름 확인하기 
```sh
git rev-parse --abbrev-ref HEAD
```

## 커밋에서 파일 하나 제외하기 (예. Changelog).
```sh
git update-index --assume-unchanged Changelog; git commit -a; git update-index --no-assume-unchanged Changelog
```

## 리베이스 하기 전에 저장하기 
```sh
git rebase --autostash
```

## 원격리파지토리의 변경사항을 로컬브랜치로 이동합니다. 
```sh
git fetch origin pull/<id>/head:<branch-name>
```


__Alternatives:__
```sh
git pull origin pull/<id>/head:<branch-name>
```

## 현재브랜치에서 가장 최근에 태깅뇐 내용 보여주기 
```sh
git describe --tags --abbrev=0
```

## 변경사항 확인하기 .
```sh
git diff --word-diff
```

## 형상관리 되는 파일의 변경사항을 변경되지 않은 것으로 표시하기 
```sh
git update-index --assume-unchanged <file_name>
```

## 변경되지 않았다고 표시된 내용을 되돌리기.
```sh
git update-index --no-assume-unchanged <file_name>
```

## 제외된 목록으로부터 필요없는 파일 삭제하기 
```sh
git clean -X -f
```

## 삭제된 파일 복구하기 
```sh
git checkout <deleting_commit>^ -- <file_path>
```

## 파일을 특정 커밋으로 되돌리기 
```sh
git checkout <commit-ish> -- <file_path>
```

## 원격리파지토리의 내용을 받아올때 머지 대신에 리베이스하기 
```sh
git config --global branch.autosetuprebase always
```

## Git 설정 모두 보기 
```sh
git config --list
```

## 대소문자 구별하도록 설정하기 
```sh
git config --global core.ignorecase false
```

## 오탈자 자동 수정하기 
```sh
git config --global help.autocorrect 1
```

## 특정 릴리즈의 변경사항이었는지 확인하기 
```sh
git name-rev --name-only <SHA-1>
```

## 모의 수행. ( 모든 명령어가 dry-run 옵션을 지원함. ))
```sh
git clean -fd --dry-run
```

## 이전 커밋을 수정했다고 현재 커밋에 표시하기 
```sh
git commit --fixup <SHA-1>
```

## 커밋과 수정된 커밋을 하나로 합치기 
```sh
git rebase -i --autosquash
```

## 커밋하는 동안 스테이지에 넣는 행동 생략하기 
```sh
git commit -am <commit message>
```

## 제외된 파일 목록 보기 
```sh
git check-ignore *
```

## 제외된 파일들의 현재상태 확인하기 .
```sh
git status --ignored
```

## 브랜치1의 커밋을 브랜치2에 커밋하기 
```sh
git log Branch1 ^Branch2
```

## 현재의 이전의 충돌 해법을 기록하고 재사용하도록 설정하기 
```sh
git config --global rerere.enabled 1
```

## 충돌이 발생한 모든 파일을 에디터에서 열기 
```sh
git diff --name-only | uniq | xargs $EDITOR
```

## 디스크를 소비하고있는 압축되지 않은 오브젝트의 갯수 세기 
```sh
git count-objects --human-readable
```

## 오브젝트 데이터페이스에서 접근할 수 없는 모든 오브젝트 제외하기 .
```sh
git gc --prune=now --aggressive
```

## 작업중인 리파지토리를 바로 웹에서 확인하기 
```sh
git instaweb [--local] [--httpd=<httpd>] [--port=<port>] [--browser=<browser>]
```

## 커밋 로그에서 GPG 서명 확인하기 
```sh
git log --show-signature
```

## 전역 설정 삭제하기 
```sh
git config --global --unset <entry-name>
```

## 파일 내용만 담고 이력을 가지지 않는 새로운 브랜치 생성하기 
```sh
git checkout --orphan <branch_name>
```

## 최종 커밋과 스테이지된 파일의 변경사항 확인하기 
```sh
git diff --staged
```

## 다른 브랜치의 파일 내용 확인하기 .
```sh
git show <banch_name>:<file_name>
```

## 루트와 머지된 커밋 목록만 확인하기
```sh
git log --first-parent
```

## 이전의 두 커밋을 하나로 합치기 
```sh
git rebase --interactive HEAD~2
```

## 현재 작업중인 브랜치 목록 보기 
```sh
git checkout master && git branch --no-merged
```

<!-- Don’t remove or change the comment below – that can break automatic updates. More info at <http://npm.im/doxie.inject>. -->
<!-- @doxie.inject end -->
