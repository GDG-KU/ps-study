# ps-study
개개인의 PS 기록을 관리하기 위해 [`git submodule`](https://git-scm.com/book/ko/v2/Git-%EB%8F%84%EA%B5%AC-%EC%84%9C%EB%B8%8C%EB%AA%A8%EB%93%88)을 사용합니다.

## How to start

```bash
# submodule이 포함된 저장소를 받아오기 위해서 --recurse-submodules 옵션 사용
git clone --recurse-submodules https://github.com/GDG-KU/ps-study.git

git submodule add [본인의 PS 저장소 URL] [Path] # 본인의 PS 저장소를 submodule로 등록합니다.
# e.g. git submodule add https://github.com/mobius29/ProblemSolving.git LeeSeongjin

git config -f .gitmodules submodule.[Path].branch main # 등록한 submodule을 저장소의 main branch를 추적하도록 합니다.
# e.g. git config -f .gitmodules submodule.LeeSeongjin.branch main
```

아래 두 사항을 확인하고 Commit & Push 진행
- `.gitmodules` 파일에 본인의 저장소가 잘 추가되었는지
- 본인의 PS Repository가 잘 Clone 되었는지

---
## References
- [깃(Git) & 깃허브(GitHub)](https://wikidocs.net/300274)
