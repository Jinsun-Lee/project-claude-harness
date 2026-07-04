# 메모리 저장
1. 메모리는 로컬 기본 위치(`~/.claude/projects/.../memory/`)가 아니라 현재 작업 중인 레포 내부 `<repo>/.claude/memory/`에 저장한다.
   1. git으로 버전관리되어 원격에 함께 올라가고 다른 머신·세션에서도 공유되도록 하기 위함이다.
2. 저장 형식은 기존 메모리 패턴을 그대로 유지한다. 사실 1개당 frontmatter(`name` / `description` / `metadata.type`)를 가진 `.md` 파일 1개 + 같은 폴더의 `MEMORY.md`에 인덱스 한 줄 추가.
3. git 레포 밖에서 작업 중이면 바탕화면의 `memory/` 폴더에 같은 패턴으로 저장한다.