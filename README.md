# Dale Design - 프로젝트 갤러리

GitHub Pages에서 실행 가능한 반응형 이미지 갤러리 웹사이트입니다.

## 🚀 주요 기능

### 1. 이미지 리스트 페이지
- 그리드 형태의 프로젝트 카드 표시
- 카테고리별 필터링 (웹디자인, 브랜딩, 인쇄물)
- 반응형 그리드 레이아웃
- 호버 효과 및 애니메이션

### 2. 상세 페이지
- 프로젝트 제목 및 설명
- 다중 이미지 갤러리 (N개 이미지 지원)
- 참여 기간, 고객사, 업종, 스타일, 메인컬러 정보
- 이미지 네비게이션 (이전/다음, 썸네일 클릭)
- 터치 제스처 지원 (모바일)

### 3. 반응형 디자인
- 데스크톱, 태블릿, 모바일 최적화
- CSS Grid와 Flexbox 활용
- 미디어 쿼리 기반 반응형 레이아웃

## 🛠️ 기술 스택

- **HTML5**: 시맨틱 마크업
- **CSS3**: Flexbox, Grid, 애니메이션, 미디어 쿼리
- **Vanilla JavaScript**: ES6+ 클래스 기반 구조
- **JSON**: 정적 데이터 관리
- **GitHub Pages**: 정적 호스팅

## 📁 프로젝트 구조

```
DaleDesign/
├── index.html              # 메인 페이지 (이미지 리스트)
├── detail.html             # 상세 페이지
├── css/
│   ├── style.css          # 메인 스타일
│   ├── responsive.css     # 반응형 스타일
│   └── detail.css         # 상세 페이지 전용 스타일
├── js/
│   ├── main.js            # 메인 페이지 로직
│   └── detail.js          # 상세 페이지 로직
├── data/
│   └── projects.json      # 프로젝트 데이터
└── README.md              # 프로젝트 설명서
```

## 🚀 실행 방법

### 1. 로컬 실행
```bash
# 프로젝트 클론
git clone [repository-url]
cd DaleDesign

# 로컬 서버 실행 (Python)
python -m http.server 8000

# 또는 Node.js
npx serve .

# 브라우저에서 접속
http://localhost:8000
```

### 2. GitHub Pages 배포
1. GitHub 저장소에 코드 푸시
2. Settings > Pages에서 소스 선택
3. 브랜치 선택 후 저장
4. `https://[username].github.io/[repository-name]`에서 접속

## 📱 반응형 브레이크포인트

- **Large Desktop**: 1200px 이상
- **Desktop**: 1199px 이하
- **Tablet**: 768px 이하
- **Mobile**: 480px 이하
- **Small Mobile**: 360px 이하

## 🎨 JSON 데이터 구조

```json
{
  "projects": [
    {
      "id": "project1",
      "title": "프로젝트 제목",
      "thumbnail": "썸네일 이미지 URL",
      "images": ["이미지1", "이미지2", "이미지3"],
      "period": "참여 기간",
      "client": "고객사",
      "industry": "업종",
      "style": "디자인 스타일",
      "mainColor": "#색상코드",
      "category": "카테고리",
      "description": "프로젝트 설명"
    }
  ]
}
```

## ✨ 주요 기능 상세

### 이미지 갤러리
- 키보드 네비게이션 (← → Home End)
- 터치 스와이프 제스처
- 썸네일 클릭으로 이미지 변경
- 이미지 카운터 표시

### 필터링 시스템
- 카테고리별 프로젝트 필터링
- 실시간 결과 업데이트
- 활성 필터 시각적 표시

### 성능 최적화
- 이미지 지연 로딩 (Lazy Loading)
- Intersection Observer API 활용
- CSS 애니메이션 최적화

## 🔧 커스터마이징

### 색상 테마 변경
`css/style.css`에서 CSS 변수 수정:
```css
:root {
  --primary-color: #667eea;
  --secondary-color: #764ba2;
  --accent-color: #50C878;
}
```

### 새로운 카테고리 추가
1. `data/projects.json`에 카테고리 추가
2. `index.html`의 필터 버튼 추가
3. `js/main.js`의 필터 로직 업데이트

### 이미지 추가/수정
`data/projects.json`의 `images` 배열에 이미지 URL 추가

## 🌟 향후 확장 계획

- [ ] 검색 기능
- [ ] 무한 스크롤
- [ ] 이미지 확대/축소
- [ ] 다크 모드
- [ ] PWA 지원
- [ ] 다국어 지원

## 📄 라이선스

이 프로젝트는 MIT 라이선스 하에 배포됩니다.

## 🤝 기여하기

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📞 문의

프로젝트에 대한 문의사항이 있으시면 이슈를 생성해주세요.

---

**Dale Design** - 창의적인 디자인 프로젝트 갤러리
