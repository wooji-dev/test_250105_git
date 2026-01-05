# Git 학습 레포지토리

이 레포지토리는 Git의 원리(내부 동작 방식)와 실무에서 Git을 사용하는 방법을 학습하기 위한 실습용 자료입니다. 기본 개념 설명과 함께 직접 명령어를 실행해보며 원리를 이해하도록 구성되어 있습니다.

## 목표

- Git의 핵심 원리 이해: 객체 모델(블롭, 트리, 커밋), 레퍼런스(refs), 인덱스(index), DAG(Commit 그래프)
- 기본 사용법 숙달: `commit`, `branch`, `merge`, `rebase`, `stash` 등
- 협업 워크플로우 이해: feature-branch, pull request, 코드 리뷰, 충돌 해결
- 로컬과 원격 저장소의 동작 이해: `fetch`, `pull`, `push`의 차이

## 구성

- `src/` : 예제 코드와 간단한 실습 스크립트
- `data.json`, `hello.txt` : 연습용 파일
- 이 `README.md` : 학습 안내서

## 시작하기 (간단한 실습)

다음은 기본적인 실습 흐름 예시입니다.

```bash
# 레포 클론
git clone <repository-url>
cd test_250105_git

# 새 브랜치 생성 및 이동
git checkout -b feature/learn-git

# 파일 수정하고 커밋
echo "학습용 변경" >> hello.txt
git add hello.txt
git commit -m "chore: 연습용 커밋"

# 원격에 푸시
git push -u origin feature/learn-git
```

## 추천 학습 순서

1. 기본 개념 읽기: commit, branch, working tree, index
2. 로컬에서 여러 커밋 만들기와 브랜치 실습
3. 머지와 리베이스 차이 실습 및 충돌 해결 연습
4. 원격 저장소와 협업 워크플로우(PR 포함) 경험하기
5. 내부 원리 학습: `.git/objects`, 커밋 그래프, 해시 함수의 역할

## 참고 자료

- Pro Git (무료 책): https://git-scm.com/book/ko/v2
- Git 공식 문서: https://git-scm.com/docs

원하시면 실습용 스크립트와 단계별 튜토리얼(명령어와 기대 결과)을 추가로 만들어드리겠습니다.
