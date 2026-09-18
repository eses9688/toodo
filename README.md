# Toodo

투두메이트가 데스크톱에서 잘 안 돌아가서 직접 만든 개인용 할 일 관리 웹앱입니다. 빌드 과정 없이 `index.html` 파일 하나로 동작하며, 로그인 시 Firebase(Firestore)를 통해 기기 간 데이터가 동기화됩니다.

**[Live Demo](https://eses9688.github.io/toodo/)**

## Features

- **날짜별 할 일 관리** — 일간/주간/월간 세 가지 뷰로 전환하며 할 일을 확인하고 관리
- **반복 할 일** — 매일 / 매주(요일 지정) / 매월 반복되는 습관성 할 일 등록
- **태그 분류** — 색상 태그를 만들어 할 일을 분류하고 태그별로 필터링
- **순서 변경** — 드래그 앤 드롭으로 할 일 목록 순서를 자유롭게 조정 (날짜별로 독립 저장)
- **다크 모드** — 시스템 설정을 자동으로 따라가며, 버튼으로 수동 전환도 가능
- **계정 & 클라우드 동기화** — 아이디/비밀번호로 회원가입하면 Firestore에 데이터가 저장되어 기기를 바꿔도 이어서 사용 가능. 로그인하지 않으면 브라우저 `localStorage`에만 저장되는 로컬 전용 모드로 동작
- **내보내기** — 현재 데이터를 JSON으로 백업 다운로드
- **관리자 페이지 (`admin.html`)** — 가입한 사용자 목록과 각자의 할 일/태그를 조회하고, 필요 시 사용자 데이터를 삭제할 수 있는 읽기 전용 관리 도구 (관리자 계정만 접근 가능하도록 Firestore 보안 규칙으로 제한)

## Tech Stack

Vanilla HTML / CSS / JavaScript — 프레임워크나 빌드 도구 없이 단일 파일로 구성했습니다. 인증/DB는 Firebase (Authentication + Firestore) Spark(무료) 플랜을 사용합니다.

## Usage

```bash
git clone https://github.com/eses9688/toodo.git
cd toodo
# index.html을 브라우저로 바로 열면 됩니다. (로그인 없이도 로컬 저장으로 전체 기능 사용 가능)
```

클라우드 동기화 기능을 직접 붙이려면 본인의 Firebase 프로젝트를 만들어 `index.html`과 `admin.html`의 `firebaseConfig` 값을 교체하고, Firestore 보안 규칙에서 본인 계정 UID를 관리자로 지정하면 됩니다.

## License

Personal project, MIT License.
