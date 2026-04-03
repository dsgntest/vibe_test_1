# Subscription Manager

Google AI Studio에서 생성한 `Vite + React + TypeScript` 앱을 GitHub Pages에 배포할 수 있도록 정리한 프로젝트입니다.

## 로컬 실행

```bash
npm install
npm run dev
```

## 빌드

```bash
npm run build
```

GitHub Pages 배포를 위해 `vite.config.ts`는 `base: './'`로 설정되어 있어 저장소 이름이 바뀌어도 정적 자산 경로가 깨지지 않습니다.

## GitHub Pages 배포

1. 이 폴더를 GitHub 저장소에 푸시합니다.
2. GitHub 저장소의 `Settings > Pages`에서 배포 소스를 `GitHub Actions`로 설정합니다.
3. `main` 브랜치에 푸시하면 자동으로 빌드 후 배포됩니다.

배포 URL 형식:

```text
https://<github-username>.github.io/<repo-name>/
```

## 참고

- 현재 앱은 정적 프론트엔드만 사용하므로 GitHub Pages에 적합합니다.
- 브라우저에 API 키를 주입하는 설정은 제거했습니다.
- 외부 로고 이미지는 일부 서드파티 도메인에서 불러오므로, 해당 서비스 응답 정책에 따라 표시가 달라질 수 있습니다.
