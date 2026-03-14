# 배포 가이드 - GitHub + Vercel

## 1단계: GitHub 저장소 만들기

1. [GitHub](https://github.com) 로그인
2. 우측 상단 **+** → **New repository** 클릭
3. Repository name: `seol-walk-beeper` (또는 원하는 이름)
4. **Public** 선택
5. **Create repository** 클릭 (README 등 추가하지 말 것)

---

## 2단계: 터미널에서 푸시하기

프로젝트 폴더에서 아래 명령어 실행:

```bash
cd /Users/bina/seol-walk-beeper

# Git 초기화
git init

# 파일 추가
git add .

# 커밋
git commit -m "Initial commit: 설이 산책 삐삐"

# GitHub 저장소 연결 (본인 username으로 변경)
git remote add origin https://github.com/YOUR_USERNAME/seol-walk-beeper.git

# 메인 브랜치 이름 설정
git branch -M main

# 푸시
git push -u origin main
```

> GitHub에 처음 푸시할 때 로그인 창이 뜨면 브라우저에서 인증하면 됩니다.

---

## 3단계: Vercel로 배포하기

1. [vercel.com](https://vercel.com) 접속 → **Sign Up** (GitHub 계정으로 로그인)
2. **Add New** → **Project** 클릭
3. **Import** 목록에서 `seol-walk-beeper` 저장소 선택
4. **Deploy** 클릭

약 1분 후 `https://seol-walk-beeper-xxxx.vercel.app` 형태의 도메인이 생성됩니다.

---

## 커스텀 도메인 (선택)

Vercel 프로젝트 → **Settings** → **Domains**에서
- `seol-walk.vercel.app` 같은 서브도메인
- 또는 본인 구입한 도메인

을 연결할 수 있습니다.
