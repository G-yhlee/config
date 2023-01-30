#### 설정

```md
# code ~/.gitconfig

- username
- email
```

#### vscode 에서 git 동작시키기

```md
git config --global core.editor "code --wait"

[참고]
https://dev.to/colbygarland/using-vs-code-to-git-rebase-1lc
```

#### 로컬에서 .gitignore 하는 방법

[방법1](https://stackoverflow.com/questions/1753070/how-do-i-configure-git-to-ignore-some-files-locally)
[방법2](https://sebastiandedeyne.com/setting-up-a-global-gitignore-file/)

```hs
# 방법 1 .git/info/exclude 파일에서 관리하기

--  프로젝트의 루트 디렉토리 ( .gitignore 파일이랑 같은 위치 ) 에서 exclude 파일을 연다
code .git/info/exclude

-- exclude 파일에 로컬에서 ignore 하고자하는 .gitignore 내용 복붙
복붙




# 방법 2. 홈 디렉토리에 .gitignore 세팅

-- 홈 디렉토리에서 내컴퓨터 전역에 .gitignore 되도록 할수 있다
방법2 링크 참조


```

#### git push 옵션들

```js
git push --force-with-lease // force 할때 옵션 주기
git push origin --delete feature/TEST-860 // 원격브랜치 삭제
```
