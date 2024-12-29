# Github 사용 정책

`tech-challenge` 저장소는 branch protection rule 설정이 있습니다.

```
`main` 브랜치는 3가지 rule을 지켜야 합니다.
```

<h3> Rules </h3>

1. Restrict deletions: 삭제 권한이 있는 사용자만 삭제를 허용
2. Require a pull request before merging: 모든 커밋은 `main` 브랜치가 아닌 브랜치에서 이루어져야 하고 병합 전 `pull request`를 통해 제출
   - 승인 리뷰 수: 1
   - `pull request`를 병합하려면 먼저 코드에 대한 모든 대화를 해결
3. Block force pushes: `push` 권한 있는 사용자가 강제 푸시하는 것을 방지

<h3> Commit Message </h3>

- 제목: `[반영날짜/접두어]` 
  - [241229/추가]
  - [241229/수정]
  - [241229/삭제]
- 설명: `텍스트 나열보다는 가독성을 위해 구분자를 사용하는 것을 권장` (아래 예시 참고)
    ```
    HTTP(Hypertext Transfer Protocol)
    - HTTP는 HTML과 같은 하이퍼미디어 문서를 전송하기 위한 애플리케이션 계층 프로토콜
    - 웹 브라우저와 웹 서버간 통신을 위해 설계
    - 기계 간 통신, API에 대한 프로그래밍 방식 접근 등 다른 목적으로도 사용
    ```

<h3> File and Directory architecture </h3>

- 알고리즘 문제 풀이: /algorithms/{문제유형}/{문제명}.ext
  - `e.g. algorithms/sorting/quicksort.ext`
    - Python: .py
    - JavaScript: .js
    - Java: .java
    - C++: .cpp
    - Kotlin: .kt
    - Go: .go
    - Swift: .swift
- 기술 지식: /knowledge/{주제}/{자료명}.md
  - `e.g. knowledge/os/kernal.md`

<h3> Code Style </h3>

- 언어별 Linter 설정 (e.g. java-google-style)
- 일관된 코드 스타일 유지
  - Google Style Guide

GitHub Google Style Guide: https://github.com/google/styleguide <br/>
IntelliJ Java Style: https://github.com/google/styleguide/blob/gh-pages/intellij-java-google-style.xml

<h3> Branch Protection Rule </h3>

- Settings → Branches
  - 소규모 프로젝트 수행할 때 느슨한 보호 규칙 제공에 적합
  - 푸시 권한이 있는 사용자 중 everyone or specify 설정이 가능
  - 기존의 제공된 보호 규칙
- Settings → Rules
  - 협력자들과 함께 대규모 프로젝트 수행할 때 강한 보호 규칙 제공에 적합
  - 푸시 권한이 있는 사용자 중 everyone or specify 설정이 불가능
  - 향상된 브랜치 보호 규칙
