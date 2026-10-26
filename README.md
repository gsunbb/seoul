# 서울 발견 탐험대 — Vercel 배포용

65개 자랑거리, 사진, 조사 노트 기능을 포함한 정적 웹사이트입니다.

## GitHub + Vercel
1. ZIP을 풀고 내용 전체를 GitHub 저장소에 올립니다. public 폴더와 vercel.json이 저장소 최상위에 있어야 합니다.
2. Vercel에서 해당 저장소를 Import 합니다.
3. Framework Preset: Other / Build Command: 비움 / Output Directory: public
4. Deploy를 누릅니다. 별도 환경 변수나 데이터베이스는 필요 없습니다.

## CLI
압축을 푼 폴더에서 `npx vercel --prod`를 실행하고 계정/프로젝트 안내를 따릅니다.

## 사용 안내
- 조사 기록은 학생 각 기기의 브라우저에 저장됩니다. 서버나 교사에게 전송되지 않습니다.
- 배포 주소가 바뀌면 기존 주소에 저장한 기록은 새 주소로 자동 이전되지 않습니다.
- 파일 더블클릭 대신 웹서버로 열어야 JSON 데이터를 불러올 수 있습니다.
- 로컬 미리보기: `python -m http.server 8000 --directory public` 실행 후 http://localhost:8000 접속
- 사진 및 자료 출처는 photos.json과 각 장소 카드에 있습니다.
- Google Fonts를 사용하며, 연결되지 않으면 기기의 기본 글꼴로 표시합니다.
- 학생 배포 전 실제 학생 기기에서 로그인 없이 접속되는지 확인하세요.

공식 배포 설정 안내: https://vercel.com/docs/builds/configure-a-build
