## ✅통합 브랜치(Integration Branch)
- 통합 브랜치란 언제든지 배포할 수 있는 버전을 만들 수 있어야 하는 브랜치
- 어플리케이션의 모든 기능이 정상적으로 동작하는 상태를 유지하는 것이 중요
- 보통 master 브랜치를 통합 브랜치로 사용


## ✅토픽 브랜치(Topic Branch)
- 기능 추가나 버그 수정과 같은 단위 작업을 위한 브랜치
- 여러 개의 작업을 동시에 진행할 때에는, 그 수만큼 토픽 브랜치를 생성
- 토픽 브랜치는 보통 통합 브랜치로부터 만들어 내며, 토픽 브랜치에서 특정 작업이 완료되면 다시 통합 브랜치에 병합하는 방식으로 진행
- 토픽 브랜치는 '피처 브랜치(Feature branch)' 라고 부르기도 함



## A successful Git branching model

### 메인 브랜치(Main branch)

master 브랜치와 develop 브랜치, 이 두 종류의 브랜치를 보통 메인 브랜치로 사용

- master
  - master 브랜치에서는, `배포 가능한 상태만`을 관리, 커밋할 때에는 태그를 사용하여 배포 번호를 기록
- develop
  - develop 브랜치는 앞서 설명한 통합 브랜치의 역할을 함. `평소에는 이 브랜치를 기반으로 개발`을 진행

### 피처 브랜치(Feature branch)
- 피처 브랜치는, 앞서 설명한 `토픽 브랜치 역할`을 담당
- `새로운 기능 개발 및 버그 수정이 필요할` 때에 'develop' 브랜치로부터 분기
- 피처 브랜치에서의 작업은 기본적으로 공유할 필요가 없기 때문에, 원격으로는 관리하지 않습니다. 개발이 완료되면 'develop' 브랜치로 병합하여 다른 사람들과 공유

### 릴리즈 브랜치(Release branch)
- 릴리즈 브랜치에서는 `버그를 수정하거나 새로운 기능을 포함한 상태`로 모든 기능이 정상적으로 동작하는지 확인
- 관례적으로 브랜치 이름 앞에 'release-' 를 붙인다. 
- 릴리즈를 위한 최종적인 버그 수정 등의 개발을 수행합니다. 모든 준비를 마치고 배포 가능한 상태가 되면 'master' 브랜치로 병합시키고, 병합한 커밋에 릴리즈 번호 태그를 추가
- 릴리즈 브랜치에서 기능을 점검하며 발견한 버그 수정 사항은 'develop' 브랜치에도 적용해 주어야 함, 그러므로 배포 완료 후 'develop' 브랜치에 대해서도 병합 작업을 수행

### 핫픽스 브랜치(Hotfix branch)

- `배포한 버전에 긴급하게 수정`을 해야 할 필요가 있을 경우, `master 브랜치에서 분기`하는 브랜치. 관례적으로 브랜치 이름 앞에 'hotfix-'를 붙인다.


---

참조

http://nvie.com/posts/a-successful-git-branching-model/