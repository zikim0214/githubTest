## 통합 브랜치(Integration Branch)
- 통합 브랜치란 언제든지 배포할 수 있는 버전을 만들 수 있어야 하는 브랜치
- 어플리케이션의 모든 기능이 정상적으로 동작하는 상태를 유지하는 것이 중요
- 보통 master 브랜치를 통합 브랜치로 사용


## 토픽 브랜치(Topic Branch)
- 기능 추가나 버그 수정과 같은 단위 작업을 위한 브랜치
- 여러 개의 작업을 동시에 진행할 때에는, 그 수만큼 토픽 브랜치를 생성
- 토픽 브랜치는 보통 통합 브랜치로부터 만들어 내며, 토픽 브랜치에서 특정 작업이 완료되면 다시 통합 브랜치에 병합하는 방식으로 진행
- 토픽 브랜치는 '피처 브랜치(Feature branch)' 라고 부르기도 함


### 메인 브랜치(Main branch)

master 브랜치와 develop 브랜치, 이 두 종류의 브랜치를 보통 메인 브랜치로 사용

- master
  - master 브랜치에서는, `배포 가능한 상태만`을 관리, 커밋할 때에는 태그를 사용하여 배포 번호를 기록
- develop
  - develop 브랜치는 앞서 설명한 통합 브랜치의 역할을 함. `평소에는 이 브랜치를 기반으로 개발`을 진행



### 피처 브랜치(Feature branch)
- 토픽 브랜치는 '피처 브랜치(Feature branch)' 라고 부르기도 합피처 브랜치는, 앞서 설명한 `토픽 브랜치 역할`을 담당


### 릴리즈 브랜치(Release branch)
릴리즈 브랜치에서는 `버그를 수정하거나 새로운 기능을 포함한 상태`로 모든 기능이 정상적으로 동작하는지 확인


### 핫픽스 브랜치(Hotfix branch)

배포한 버전에 긴급하게 수정을 해야 할 필요가 있을 경우, master 브랜치에서 분기하는 브랜치. 관례적으로 브랜치 이름 앞에 'hotfix-'를 붙인다.