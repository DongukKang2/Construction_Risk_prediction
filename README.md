# 스마트건설 구성기술3 Github 
## ■ 구성기술 3 프로세스 및 코드 번호
![image](https://user-images.githubusercontent.com/74308155/236133083-7221eccc-2ab2-4c26-ab11-632d81c7f61c.png)

## ■ VSCode 연동
1. **Git 설치**: <br> 시스템에 Git이 설치되어 있는지 확인합니다. 그렇지 않은 경우 https://git-scm.com/ 에서 다운로드하여 설치할 수 있습니다.
2. **VSCode 설치**: <br> 아직 다운로드하지 않은 경우 https://code.visualstudio.com/ 에서Visual Studio Code를 다운로드하여 설치해야 합니다.
3. **Git 구성**: <br> Git을 설치한 후 Git에서 커밋할 때 식별하는 데 사용되는 사용자 이름과 이메일 주소를 구성해야 합니다. 터미널/명령 프롬프트에서 다음 명령을 실행하여 이를 수행할 수 있습니다.

```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```
`Your Name` 및 `youremail@example.com`을 실제 이름과 이메일 주소로 바꿔야 합니다.


4. **리포지토리 복제**:<br> GitHub 리포지토리 페이지로 이동하여 "Code" 버튼을 클릭하고 URL을 복사해야 합니다. 그런 다음 터미널/명령 프롬프트를 열고 원하는 상위 폴더로 이동한 후 다음 명령을 실행해야 합니다.

```bash
git clone repository_url
```

`repository_url`을 GitHub에서 복사한 URL로 바꿔야 합니다. 이 명령은 프로젝트 파일과 .git 폴더를 포함하는 리포지토리 이름으로 새 폴더를 만듭니다.


5. **VSCode에서 복제된 리포지토리 열기**: <br>리포지토리를 복제한 후 VSCode를 열고 "파일" 메뉴에서 "폴더 열기"를 선택하거나 시작 페이지에서 "폴더 열기" 버튼을 사용할 수 있습니다. 복제된 리포지토리 폴더로 이동하여 "열기"를 클릭해야 합니다.
6. **개발 환경 설정**: <br>VSCode에서 리포지토리를 열면 개발 환경을 설정하고 필요한 종속성을 설치하고 코드 작업을 시작할 수 있습니다.
7. **공동 작업 및 파일 편집**:<br> 이제 파일을 편집하고, 변경 사항을 저장하고, VSCode의 통합 Git 기능을 사용하여 분기를 생성하고, 변경 사항을 커밋하고, 업데이트를 푸시 및 풀하고, 풀 요청을 생성할 수 있습니다. 이렇게 하면 공유 저장소에서 팀과 협업할 수 있습니다

## ■ GitHub 사용법

### Github 명령어

1. **Commit**: <br> 커밋은 특정 시점에서 작업 디렉토리의 스냅샷입니다. 여기에는 마지막 커밋 이후 파일에 적용된 변경 사항에 대한 기록이 포함됩니다. 커밋할 때 고유 식별자(해시) 및 변경 사항을 설명하는 커밋 메시지와 함께 Git 리포지토리에 로컬로 변경 사항을 저장합니다. 커밋을 사용하면 프로젝트 기록을 추적하고 필요한 경우 이전 버전으로 되돌릴 수 있습니다.

```python
git add .  # 변경사항 추적
git commit -m "Your commit message"
```

2. **Push**: <br> 푸시는 로컬 커밋을 원격 저장소(예: GitHub, GitLab, Bitbucket)에 업로드하는 행위를 의미합니다. 변경 사항을 푸시하면 로컬 리포지토리를 원격 리포지토리와 동기화하여 다른 공동 작업자가 커밋 및 변경 사항을 사용할 수 있습니다. 푸시는 브랜치 및 태그에 대한 참조도 업데이트합니다.


```bash
git push remote_name branch_name
```
`remote_name`의 기본 값은 `origin` <br>
`branch_name`의 기본 값은 `main`

3. **Pull**:<br> 풀링은 원격 리포지토리에서 변경 사항을 가져와 로컬 리포지토리에 병합하는 프로세스입니다. 풀링할 때 원격 저장소에서 새 커밋과 업데이트를 다운로드하고 이를 로컬 브랜치에 통합하여 로컬 저장소를 원격 저장소와 동기화 상태로 유지합니다.


```bash
git pull remote_name branch_name
```

4. **Pull Request**: <br> 풀 요청(GitLab의 병합 요청이라고도 함)은 GitHub, GitLab 및 Bitbucket과 같은 플랫폼에서 사용되는 협업 기능입니다. 한 브랜치의 변경 사항을 원격 저장소의 다른 브랜치로 병합하도록 요청하는 방법입니다. 풀 요청을 사용하면 변경 사항을 통합하기 전에 코드 검토, 토론 및 협업이 가능합니다. 풀 요청이 생성되면 다른 팀원은 제안된 변경 사항을 검토하고, 의견을 남기고, 수정 사항을 제안하거나 변경 사항을 승인할 수 있습니다. 검토 프로세스 후 변경 사항을 대상 브랜치에 병합할 수 있습니다.

### Github 에 파일 업로드 OR 업데이트 시

1. **터미널 Open 및 SmartConstruction_Risk 디렉토리로 이동**

2. **변경사항 추적 및 커밋**

```python
git add .  # 변경사항 추적
git commit -m "변경내용 입력" # ex) "add code 1",  "update code 1(~ 수정)"
```

3. **업로드 및 업데이트 내용 푸시**

```bash
git push remote_name branch_name
```
`remote_name`의 기본 값은 `origin` <br>
`branch_name`의 기본 값은 `main`

### Github 변경사항을 개인 vscode에 덮어쓰기

1. **터미널 Open 및 SmartConstruction_Risk 디렉토리로 이동**

2. **변경 사항 vscode에 풀**

```bash
git pull remote_name branch_name
```
`remote_name`의 기본 값은 `origin` <br>
`branch_name`의 기본 값은 `main`

## ■ 추후 버전관리를 위해 기본 브랜치인 main에서 버전관리를 위해 추가할 예정
변경테스트_종호
