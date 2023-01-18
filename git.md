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

[참고링크](https://stackoverflow.com/questions/1753070/how-do-i-configure-git-to-ignore-some-files-locally)

```hs
# 방법 1 .git/info/exclude 파일에서 관리하기

--  프로젝트의 루트 디렉토리 ( .gitignore 파일이랑 같은 위치 ) 에서 exclude 파일을 연다
code .git/info/exclude

-- exclude 파일에 로컬에서 ignore 하고자하는 .gitignore 내용 복붙
복붙




# 방법 2. 홈 디렉토리에 .gitignore 세팅

-- 홈 디렉토리에서 내컴퓨터 전역에 .gitignore 되도록 할수 있다
-- 아직 해보진 않음



```
