# Company Work Automation

Recreated workplace solutions and practical tools for everyday workflow automation.

반복적인 업무에서 출발한 자동화 도구를 공개용으로 정리하는 개인 포트폴리오 저장소입니다. 회사 운영 환경과 분리하여 관리합니다.

## Tools

| 도구 | 해결하는 문제 | 주요 기술 |
| --- | --- | --- |
| [공공 통계 갱신일 확인](public-data-update-checker/) | 여러 공공 통계의 원천 갱신일을 한 번에 조회하고 최신 확인 상태 저장 | Python, Requests, Beautiful Soup, KOSIS Open API, CSV |

### Public Data Update Checker

index.go.kr 4개 지표와 KOSIS 12개 통계표를 확인하는 Jupyter 노트북입니다.

- HTML과 API 응답에서 갱신일 추출
- 요청 오류 및 날짜 미발견 상태 구분
- 지표별 최신 확인 결과를 CSV로 저장

회사 내부 DB 적재 여부는 검사하지 않습니다. 실행 방법과 구현 범위는 [도구 README](public-data-update-checker/README.md)를 참고하세요.

## Configuration

인증키는 환경변수로 전달합니다. 실제 키, 실행 결과 CSV, 개인 경로가 포함된 출력은 저장소에 포함하지 않습니다. 도구를 추가할 때는 별도 폴더에 코드, 실행 방법, 해결한 문제와 한계를 함께 기록합니다.
