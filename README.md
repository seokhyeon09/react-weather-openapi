# react-weather-openapi (실시간 날씨 앱)

OpenWeather API를 활용하여 실시간 기상 정보를 제공하는 동적 웹 애플리케이션입니다.

## Links
- 배포 주소: https://react-weather-openapi.vercel.app/
- GitHub 저장소: https://github.com/seokhyeon09/react-weather-openapi

## Tech Stack (사용 기술)
- Framework 및 빌드 도구: React, Vite
- Data Fetching 및 API: Axios, OpenWeather API
- State Management 및 최적화: React Hooks (useState, useEffect, useRef, useMemo)
- 보안 및 설정: Environment Variables (.env)

## Key Features (주요 기능)
- 실시간 기상 데이터 연동: axios를 활용하여 OpenWeather API와 비동기 통신을 수행하고, 현재 온도, 습도 등 핵심 기상 데이터를 빠르고 안정적으로 화면에 출력합니다.
- 날씨 맞춤형 동적 UI 렌더링: API로 받아온 날씨 상태(weather ID)를 기반으로 useMemo Hook을 활용해 화면의 배경 이미지가 즉각적으로 변하도록 구현하여 시각적인 직관성을 높였습니다.
- 컴포넌트 모듈화: 기능과 UI 요소들을 개별 파일로 분리하고 export와 import를 활용해 조합함으로써, 코드의 가독성을 개선하고 향후 다른 프로젝트에서도 재사용할 수 있도록 구조화했습니다.
- 환경 변수를 활용한 보안 관리: OpenWeather API Key와 같은 민감한 인증 정보는 하드코딩하지 않고 Vite의 환경 변수(.env) 파일로 분리했습니다. 이를 통해 깃허브(Git)와 같은 공개 저장소에 키가 노출되는 것을 방지하여 보안성을 크게 강화했습니다.

## 느낀점 / 개선할 점
- 실제 서비스처럼 외부 데이터를 다루고 최적화하는 과정을 경험할 수 있었습니다. 특히 .env 파일에 API 키를 분리하고 .gitignore를 통해 Git 추적에서 제외하는 과정을 직접 구현해 보며, 프론트엔드 환경에서의 데이터 보안과 환경 변수 관리의 중요성을 확실하게 깨달았습니다.

## Getting Started (로컬 실행 방법)

1. 저장소 클론 (Clone the repository)
git clone https://github.com/seokhyeon09/react-weather-openapi

2. 패키지 설치 (Install dependencies)
npm install

3. 개발 서버 실행 (Run the dev server)
npm run dev
