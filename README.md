# 재무제표 시각화 웹사이트

OpenDART API를 활용한 기업 재무제표 시각화 웹사이트입니다.

## 🚀 기능

- 기업 종목 검색 및 선택
- 재무제표 데이터 시각화
- 차트 및 그래프 표시
- 반응형 웹 디자인

## 🛠️ 기술 스택

- React 18 + TypeScript
- Vite
- Tailwind CSS
- Recharts (차트 라이브러리)
- Axios (HTTP 클라이언트)
- OpenDART API

## 📦 설치 및 실행

### 로컬 개발

```bash
# 의존성 설치
npm install

# 개발 서버 실행
npm run dev

# 빌드
npm run build
```

## 🌐 배포 방법

### Vercel 배포 (추천)

1. **Vercel CLI 설치**
   ```bash
   npm i -g vercel
   ```

2. **Vercel 로그인**
   ```bash
   vercel login
   ```

3. **프로젝트 배포**
   ```bash
   vercel
   ```

4. **환경 변수 설정**
   - Vercel 대시보드에서 프로젝트 선택
   - Settings > Environment Variables
   - `VITE_OPENDART_API_KEY` 추가

### GitHub 연동 배포

1. **GitHub에 코드 푸시**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/yourusername/your-repo.git
   git push -u origin main
   ```

2. **Vercel에서 GitHub 연동**
   - [vercel.com](https://vercel.com) 접속
   - "New Project" 클릭
   - GitHub 저장소 선택
   - 환경 변수 설정 후 배포

## 🔧 환경 변수

`.env` 파일에 다음 변수를 설정하세요:

```env
VITE_OPENDART_API_KEY=your_api_key_here
VITE_OPENDART_API_URL=https://opendart.fss.or.kr/api
```

## 📁 프로젝트 구조

```
src/
├── components/
│   ├── Header.tsx
│   ├── SearchSection.tsx
│   └── FinancialDataDisplay.tsx
├── services/
│   └── opendartApi.ts
├── App.tsx
└── main.tsx
```

## 🎯 사용법

1. 전체 종목 선택 드롭다운에서 원하는 기업 선택
2. 기준년도 선택 (2020-2024)
3. 보고서 유형 선택 (사업보고서, 반기보고서 등)
4. "재무제표 조회" 버튼 클릭
5. 재무 데이터 및 차트 확인

## 📄 라이선스

MIT License
