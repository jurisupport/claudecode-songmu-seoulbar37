# 클로드코드로 송무하기 — 서울지방변호사회 「자투리 시간으로 실력 UP!」 제37회 실습 자료

> 2026. 11. 18. · 로피드 법률사무소 하희봉 변호사
> 강의에서 쓰는 가상사건 기록, 사건별 꿀팁 실습 예시, 홍보 콘텐츠 실습용 판결입니다. 가상사건과 꿀팁 예시의 인물·사건·계좌·주소는 허구입니다. 홍보 콘텐츠 실습의 판결은 공개된 실제 판결입니다.

## 무엇이 들어 있나

| 폴더 | 내용 |
|---|---|
| `강의슬라이드.pdf` | 강의 슬라이드(유튜브 강의영상판, 56쪽). 웹에서 보기: https://jurisupport.github.io/claudecode-songmu-seoulbar37/강의슬라이드.pdf |
| `청중핸드아웃.html` | 강의 지시문 모음(실습사건 받기·송무 5단계·사건별 꿀팁·지시문 10개·제출 전 검수표). 지시문마다 복사 버튼이 있다. 내려받아 브라우저로 연다 |
| `실습사건_대여금/` | 시연용 가상사건 기록(김민철 vs 이정숙, 서울중앙지방법원 2026가단512345 대여금) PDF 12개와 작업 규칙 예시 `CLAUDE.md`(jurisupport-plugins `templates/사건폴더_CLAUDE.md`와 같은 파일). 이 폴더에서 Claude Code를 열면 CLAUDE.md를 먼저 읽는다 |
| `실습_꿀팁예시/` | 사건별 꿀팁(민사·형사·가사·공통) 지시문을 시험해 볼 가상 자료와 빈 서식. 공통 폴더에는 이름 없는 서증 스캔 6개와 준비서면 초안이 있다. 자세한 내용은 폴더 안 README |
| `실습_홍보콘텐츠/` | 홍보 콘텐츠 실습용 실제 판결 전문(대법원 2026. 7. 22. 선고 2022도5937 전원합의체 판결, 국가법령정보센터 원문 그대로)과 영상 시험용 8컷 컷시트(`바로시험_영상/cuts.json`). 판결은 저작권법 제7조 제3호에 따라 저작권 보호 대상이 아니다 |

## 받기

Claude Code 데스크톱 앱의 Code 탭에 아래 문장을 붙여 넣으면 됩니다.

```
github.com/jurisupport/claudecode-songmu-seoulbar37 저장소에서 세 폴더를 지금 작업 중인 폴더 안에 하위 폴더로 내려받아줘. ① 「실습사건_대여금」 폴더의 PDF 12개와 CLAUDE.md는 「실습_대여금사건」 폴더로 ② 「실습_꿀팁예시」와 ③ 「실습_홍보콘텐츠」 폴더는 통째로 같은 이름으로. 다 받으면 폴더별 파일 목록을 보여줘.
```

터미널 없이 받으려면 이 페이지 위쪽 초록색 `Code` 버튼 → `Download ZIP` → 압축을 풉니다. Windows에서 ZIP을 풀면 한글 폴더명이 깨질 수 있습니다. 그때는 위 문장으로 받으세요.

## 강의에서 소개한 스킬

모두 아래 「도구 설치」 문장 하나로 함께 설치됩니다.

| 스킬 | 하는 일 | 저장 위치 |
|---|---|---|
| korean-law (MCP) | 법령·조문·판결 원문 조회 | [korean-law-mcp](https://github.com/chrisryugj/korean-law-mcp) |
| legal-books | 사무소 보유 교과서 검색(저자·서명·판차·쪽수 인용) | [legal-books](https://github.com/jurisupport/legal-books) |
| legal-calc | 기간 만료일·일수·지연손해금 계산 | [plugins/jurisupport/skills/legal-calc](https://github.com/jurisupport/jurisupport-plugins/tree/main/plugins/jurisupport/skills/legal-calc) |
| privacy-consent-interview | 개인정보 처리방침·동의서 초안 문답 | [plugins/jurisupport/skills/privacy-consent-interview](https://github.com/jurisupport/jurisupport-plugins/tree/main/plugins/jurisupport/skills/privacy-consent-interview) |
| law-forms | 법령·법원 서식(hwpx) 채우기 | [skills/law-forms](https://github.com/jurisupport/jurisupport-plugins/tree/main/skills/law-forms) |
| promo-content | 판결 → 블로그·쇼츠 원고·컷시트·SNS 글, 광고 규정 점검 | [plugins/jurisupport/skills/promo-content](https://github.com/jurisupport/jurisupport-plugins/tree/main/plugins/jurisupport/skills/promo-content) |
| explainer-video | 컷시트 → 설명 영상 | [plugins/jurisupport/skills/explainer-video](https://github.com/jurisupport/jurisupport-plugins/tree/main/plugins/jurisupport/skills/explainer-video) |
| narration-shorts | 쇼츠 원고 → 내레이션 쇼츠 | [plugins/jurisupport/skills/narration-shorts](https://github.com/jurisupport/jurisupport-plugins/tree/main/plugins/jurisupport/skills/narration-shorts) |
| legal-polish-public | 법률문서 문장 다듬기 | [legal-polish-public](https://github.com/jurisupport/legal-polish-public) |

핸드아웃에서 「강사 PC」로 표시한 지시문은 강사 PC의 개인 스킬로 시연한 것입니다. 이 스킬들은 공개 묶음에 들어 있지 않습니다.

## 도구 설치

플러그인·스킬 설치는 https://github.com/jurisupport/jurisupport-plugins 를 따릅니다.
