# Toodo

투두메이트가 데스크톱에서 잘 안 돌아가서 직접 만든 개인용 할 일 관리 웹앱입니다. 빌드 과정이나 서버 없이 `index.html` 파일 하나로 동작합니다.

**[Live Demo](https://eses9688.github.io/toodo/)**

## Features

- **날짜별 할 일 관리** — 일간/주간/월간 세 가지 뷰로 전환하며 할 일을 확인하고 관리
- **반복 할 일** — 매일 / 매주(요일 지정) / 매월 반복되는 습관성 할 일 등록
- **태그 분류** — 색상 태그를 만들어 할 일을 분류하고 태그별로 필터링
- **순서 변경** — 드래그 앤 드롭으로 할 일 목록 순서를 자유롭게 조정 (날짜별로 독립 저장)
- **다크 모드** — 시스템 설정을 자동으로 따라가며, 버튼으로 수동 전환도 가능
- **로컬 저장** — 서버 없이 브라우저 `localStorage`에 데이터 저장, JSON으로 내보내기(백업) 지원

## Tech Stack

Vanilla HTML / CSS / JavaScript — 프레임워크나 빌드 도구 없이 단일 파일로 구성했습니다.

## Usage

```bash
git clone https://github.com/eses9688/toodo.git
cd toodo
# index.html을 브라우저로 바로 열면 됩니다.
```

## License

Personal project, MIT License.
