# 💜 Dearie
팬 활동 기록 및 아티스트 커뮤니티 인터랙션 웹 애플리케이션

Dearie는 팬 활동을 기록하고, 아티스트 게시글 열람 및 팬 간의 커뮤니티 인터랙션 경험을 제공하는 React 기반 웹 애플리케이션입니다.

🌐 Live Demo
https://dearie-app-v3.vercel.app/

---

## 📌 프로젝트 개요

| 항목 | 내용 |
|------|------|
| 프로젝트명 | Dearie |
| 개발 기간 | 2025.07.01 ~ 2025.07.30 (약 4주) |
| 개발 인원 | 6명 |
| 개발 방식 | Frontend Web Application |

---

## 🛠 기술 스택

**Frontend**
- React 19
- JavaScript (ES6+)
- React Router DOM v7
- Swiper.js / Framer Motion

**Styling**
- CSS3 / Flexbox / Grid

**Version Control**
- Git / GitHub

**배포**
- Vercel

---

## ✨ 주요 기능

**👤 아티스트 페이지**
- 아티스트 프로필 및 게시글 조회
- 게시글 좋아요 기능

**💬 Talk 섹션**
- 유저 게시글 작성 / 수정 / 삭제
- 아티스트 + 유저 게시글 통합 피드
- 댓글 작성 / 삭제 / 좋아요 / 신고

**🖼 이미지 업로드**
- Canvas API 기반 이미지 리사이즈 및 base64 저장

**📌 기타**
- 탭 상태 유지
- 팬레터 (To.) 조회
- 하이라이트 섹션

---

## 👩‍💻 프로젝트에서의 역할

담당 파트: **아티스트 페이지**

### 🎯 Frontend

**React 기반 아티스트 페이지 구조 설계 및 구현**
- 아티스트페이지 4개 섹션(Highlight / Artist / Talk / Content) 및 상세 페이지 전체 구현
- 탭 컴포넌트를 배열로 관리해 확장성 확보, 탭 상태를 localStorage에 저장해 뒤로가기 후 복원 구현

**Talk 섹션 게시글 CRUD 구현**
- 유저 게시글 작성 / 수정 / 삭제 기능 구현
- 수정 시 sessionStorage로 기존 글 데이터를 작성 페이지에 전달, 사용 후 즉시 삭제

**댓글 기능 구현**
- localStorage에 저장된 고유 userId로 내 댓글만 삭제 가능하도록 처리
- 댓글 좋아요 / 신고 기능 구현

### 🎨 UI/UX

- CSS3 / Flexbox / Grid 기반 반응형 UI 구현
- 1분 단위 자동 리렌더링으로 시간 표시 실시간 갱신 (`N분 전`, `N시간 전` 등)

---

## 🔧 개선 사항

- 유저 인증 기능 추가 (JWT) — 현재 localStorage userId로 대체 중
