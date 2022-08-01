# 목차
- [1️⃣ clone](#clone)
- [2️⃣ fork](#fork)
- [3️⃣ clone vs fork](#clone-vs-fork)

# ✔CLONE
- git clone https://github.com/myungyi0314/githubTest.git
- Github Repository에 있는 프로젝트를 내 컴퓨터로 가져오는 것(remote를 local로)


![1 Git Clone](https://user-images.githubusercontent.com/52149400/181718466-c9e5e046-2337-49e1-b2bf-76e723c75a90.png)

![2 Git Clone - Cloning a Repo](https://user-images.githubusercontent.com/52149400/181718483-3b725868-e657-475c-92f0-68af5a2298b3.png)



# ✔FORK
- 남이 만든 Repository를 그대로 복사해서 내 GitHub 계정으로 가져오는 것
- 가져오면서 Repository명 변경 가능
- 컴퓨터의 한 드라이브에서 다른 드라이브로 폴더를 복사하는 것과 유사
- 사용자는 이 리포지토리를 자신의 목적을 위해 자유롭게 사용하거나 코드 변경을 실험할 수 있습니다. git forking을 통해 사용자는 다른 사람의 코드에 대한 수정 사항을 직접 개발
- 원래 저장소( 업스트림 저장소라고도 함 ) 코드 에는 영향을 미치지 않습니다 .
- 저장소와 코드는 사용자의 GitHub 계정으로 제한 사용자의 로컬이나 프로세스에서 git의 참여에는 영향이 없다.

![1 Git Fork - Fork a Repo](https://user-images.githubusercontent.com/52149400/181720220-7c813096-99f2-4cb6-97cb-721c8a52d127.png)

## FORK를 하는 이유?
GitHub는 전 세계 모든 개발자에게 플랫폼을 제공하여 서로의 
프로젝트에 기여하고 더 좋고 더 안정적인 소프트웨어를 만들 수 있도록 개발되었습니다. 
아무도 원본 저장소에 대한 동의 없이 수백 가지 변경 사항을 보고 싶어하지 않을 것이 분명합니다. 
따라서 저장소의 복사본 또는 분기된 저장소의 개념이 등장

1. Upstream Repository의 코드 or 소프트웨어 개선
   *  Repositroy를 분기하고 버그, 실행시간 개선, 새로운 기능을 추가하여 해당 변경 사항을 repository소유자에게 보낼 수 있다.
2. 내 프로젝트에서 코드 재사용 
   * 다른 사람의 저장소를 분기해서 내 프로젝트에서 사용 할 수도 있다.
## FORK 순서
1. repository fork
2. code 변경
   - git clone
4. 원본 repo로 변경사항 보내기 
   - pull request 사용자 변경 사항을 수락하기 위해 업스트림 저장소 소유자에게 요청을 함


> pull request 란? <br>
> 내가 수정한 코드가 있으니 내 branch를 가져가 검토 후 병합해주세요 라는 뜻 <br>
> 코드 충돌을 최소화할 수 있고 push 권한이 없는 <br>
> 오픈 소스 프로젝트에 기여할 때 많이 사용 

![2 1_Pull-Request](https://user-images.githubusercontent.com/52149400/181720241-529bc623-d7c9-42fe-9c9d-882e19848576.png)

# ✔CLONE VS FORK
- Fork는 GitHub 계정에서 수행되고 복제는 Git을 사용하여 수행
- 리포지토리를 분기할 때 원본 리포지토리(업스트림 리포지토리)의 복사본을 생성하지만 리포지토리는 GitHub 계정에 남아 있다. 
- 저장소를 복제하면 저장소가 Git의 도움으로 로컬 시스템에 복사

![1 Difference-between-Git-Clone-and-Git-Fork](https://user-images.githubusercontent.com/52149400/182065615-4834217e-de45-4e22-a1d9-3a8f43f18cca.png)

- 포크된 리포지토리에 대한 변경 사항은 pull 요청 을 통해 원래 리포지토리와 병합
- 반면에 로컬 시스템(복제된 저장소)에서 수행된 변경 사항은 업스트림 저장소로 직접 푸시될 수 있습니다. 
- 이 경우 복제된 저장소의 변경 사항이 먼저 분기된 저장소로 푸시된 다음 풀 요청이 생성됩니다. 

![2 Difference-between-Git-Cloning-and-Git-Forking](https://user-images.githubusercontent.com/52149400/182066510-21f4752f-681f-4854-85de-126a3dc04dc8.png)

# ✔Origin vs Upstream.
- fork의 의미에서 이해해야함
- 내가 다른 사람의 Repository를 fork 해온다면 upstream은 그 사람의 Repository(오리지널 Repository)를 의미한다.
- origin은 나의 fork이다. Repository가 clone될 때 default remote는 origin이라고 불린다. 즉, 내 fork를 myungyirepo라고 할 때, clone하면 내 repository가 origin이 된다. 
- 내 래포가 myRepo이고 다른 레포가 otherRepo라고 한다면, otherRepo로부터 pull from 해오고(당겨오고) push to한다면 내 myRepo가 downstream, otherRepo가 upstream으로 정의
- 하나의 Upstream 여러 개의 Downstream

---
### [🔼 위로](#목차)

이미지 출처-https://www.toolsqa.com/

https://www.toolsqa.com/git/git-fork/

https://velog.io/@parkirae/git-fork-%ED%95%98%EA%B1%B0%EB%82%98-clone-%ED%95%98%EA%B1%B0%EB%82%98

https://dev-youngjun.tistory.com/47

https://velog.io/@zansol/Pull-Request-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0
