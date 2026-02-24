# Snowball

Android/iOS 투자 관리 앱 — Kotlin Multiplatform 기반

## Architecture

![Architecture](./docs/architecture.svg)

## Screenshots

<img src="./docs/home_screenshot.png" width="250" alt="Home"> <img src="./docs/account_screenshot.png" width="250" alt="Account"> <img src="./docs/backtest_screenshot.png" width="250" alt="Backtest">

## Module Structure

| 모듈 | 역할 |
|------|------|
| `:app` | 앱 진입점 · DI 설정 |
| `:navigation` | 화면 전환 · Back Stack 관리 (Decompose) |
| `:feature:home` | 포트폴리오 · 투자 현황 |
| `:feature:account` | 계좌 관리 |
| `:feature:backtest` | 백테스트 엔진 · 결과 차트 |
| `:feature:detail` | 종목 상세 · 가격 히스토리 |
| `:core:ui` | 공통 UI 컴포넌트 · 테마 |
| `:core:domain` | 비즈니스 로직 · UseCase |
| `:core:data` | 데이터 접근 · Repository · Ktor |
| `:snowball-models` | 공유 데이터 모델 |

## Tech Stack

- **UI** — Compose Multiplatform · Material3
- **Navigation** — Decompose · Essenty
- **DI** — Koin
- **Network** — Ktor Client
- **Async** — Kotlin Coroutines · Flow
- **Serialization** — kotlinx-serialization
- **Image** — Coil3
