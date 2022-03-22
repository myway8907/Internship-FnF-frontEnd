# F&F Dashboard Project
- **F&F는 MLB, Discovery 등의 브랜드를 판매 유통하는 패션 기업입니다.**
- **현재 판매 현황을 분석하고 향후 전략 수립에 참고가 될 수 있도록 사내 직원 활용 용도의 비즈니스 대시보드를 개발하는 프로젝트를 진행했습니다.**
- **회사의 판매 현황 통계 데이터를 제공받아, 라이브러리 등을 활용하여 데이터 시각화 웹 페이지를 구현했습니다.**

### Members
- [윤종호](https://github.com/myway8907)
- 김정현
- 이석호
- 옥채현

## Skills
<img alt="react" src="https://img.shields.io/badge/React-06B4F8?style=for-the-badge&logo=react&logoColor=FFFFFF" /> <img alt="router" src="https://img.shields.io/badge/React Router-CA4245?style=for-the-badge&logo=React Router&logoColor=white" /> <img alt="cra" src="https://img.shields.io/badge/Create React App-09D3AC?style=for-the-badge&logo=Create React App&logoColor=white" /> <img alt="javascript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=JavaScript&logoColor=black" /> <img alt="html" src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=HTML5&logoColor=FFFFFF" /> <img alt="css" src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=CSS3&logoColor=FFFFFF" /> <img alt="styled-components" src="https://img.shields.io/badge/styled--components-DB7093?style=for-the-badge&logo=styled-components&logoColor=FFFFFF" />
### State Management
<img alt="recoil" src="https://img.shields.io/badge/Recoil-C70039?style=for-the-badge" />

### Network Request
<img alt="axios" src="https://img.shields.io/badge/Axios-FFC300?style=for-the-badge" />

### Code
<img alt="eslint" src="https://img.shields.io/badge/ESLint-4B32C3?style=for-the-badge&logo=ESLint&logoColor=white" /> <img alt="prettier" src="https://img.shields.io/badge/Prettier-F7B93E?style=for-the-badge&logo=Prettier&logoColor=black" />

### VCS
<img alt="git" src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=Git&logoColor=white" /> <img alt="github" src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=GitHub&logoColor=white" />

### Communication
<img alt="zoom" src="https://img.shields.io/badge/Zoom-2D8CFF?style=for-the-badge&logo=Zoom&logoColor=white" /> <img alt="notion" src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=Notion&logoColor=white" /> <img alt="slack" src="https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=Slack&logoColor=white" /> <img alt="trello" src="https://img.shields.io/badge/Trello-0052CC?style=for-the-badge&logo=Trello&logoColor=white" /> <img alt="teams" src="https://img.shields.io/badge/Teams-6264A7?style=for-the-badge&logo=Microsoft Teams&logoColor=white" />

### Library
<img alt="mui" src="https://img.shields.io/badge/MUI-007FFF?style=for-the-badge&logo=MUI&logoColor=white" /> <img alt="recharts" src="https://img.shields.io/badge/Recharts-C70039?style=for-the-badge" /> <img alt="datepicker" src="https://img.shields.io/badge/React--DatePicker-DE4F4F?style=for-the-badge" />

## 구현 내용
### 통계 데이터 필터 컨트롤 Nav Bar
![image](https://user-images.githubusercontent.com/93215875/159464332-bdc2f0fc-b0ca-44ea-b4bd-4350684ebb03.png)
![카테고리 데이터 조회](https://user-images.githubusercontent.com/93215875/159465354-4024c539-12f1-4eb0-ba6e-177310bba47b.gif)


✔️ `**실적 기간` / `특정 주간` / `카테고리 & 서브카테고리 구조의 제품군 선택` / `검색버튼`**

✔️ `**async / await, promise` 등을 활용한 비동기 작업 처리**

✔️ **날짜 선택 컴포넌트, 체크리스트 및 체크 요소 컴포넌트 `재사용 지향`**

✔️ `**삼항 연산자` 및 `논리 연산자`를 사용한 React 컴포넌트의 조건부 렌더링 지향**

✔️ `**Styled-components`를 활용한 레이아웃 및 스타일링 구성**

✔️ `**React-datepicker` API를 사용하여 날짜 관련 옵션 구성 및 선택 정보 props 통해 전달**

✔️ `**Dropdown 방식 체크 리스트 구성**`

- **단일 및 다중 선택 방식의 체크리스트 2종류 구현**
- **하위 선택 옵션인 `서브카테고리`의 경우, `카테고리` 옵션이 선택 되어야만 체크리스트가 표시되도록 조건부 렌더링 방식으로 구성**
- `**All` (전체 선택) 체크 기능을 넣어 사용자의 옵션 선택 로직 구성**

✔️ `**커스텀 훅 작성**`

- **옵션 선택 state 내용을 쿼리스트링으로 변환**
- **변환한 쿼리스트링을 별도의 state로 관리**
- **커스텀 훅은 필터 옵션 선택 state를 의존성 요소로 지정하여 운영**

✔️ `**검색버튼의 데이터 요청 이벤트 구현**`

- **백엔드 API 17개 → 각 API 마다 엔드포인트 구별**
- **처음 데이터 요청 시 모든 API에게 데이터 요청**
    - 대시보드에는 다양한 주제의 통계 데이터가 존재 → 다른 주제의 통계 자료를 원할 때, 전환 할 때 마다 새로운 통계 데이터를 다운받는다면 소요 시간이 발생
    - 처음 데이터 요청 시 전체 데이터를 다운받아 state에 저장
    - 사용자가 원하는 주제의 차트 및 테이블 선택 시, 미리 다운받아 저장한 통계 데이터를 가져와 화면에 시각화 자료 즉시 렌더링
- **백엔드 팀원과 API 컨벤션 합의**
- **백엔드 서버 API 주소와 쿼리스트링을 함께 사용하여 버튼 클릭 시 해당 주소로 데이터 요청**

✔️ `**useLocation`를 활용하여 웹페이지에 따라 Nav Bar 내용 변화**

- 카테고리, 스타일랭킹이라는 이름의 2개 페이지를 구현
- 각 페이지의 URL 주소에 따라 활성화되는 Nav bar의 컴포넌트 종류를 변경
### 주간 판매 현황 웹페이지 구현
![채널유통선택하기](https://user-images.githubusercontent.com/93215875/159464922-45e42701-556c-46f0-9f4a-bc24d5e7cf20.gif)


✔️ `**Recharts.js 라이브러리를 활용한 차트 시각화 자료 구성**`

✔️ `**Material-UI table을 활용한 테이블 시각화 자료 구현**`

✔️ **Recoil을 활용한 React 전역상태 관리**

- 백엔드 API를 통해 전달받은 매출 관련 통계 데이터를 전역상태로 저장 및 관리
- 회사 매출 관련 17가지 통계 자료를 객체 내부의 key 값으로 분류하여 저장

✔️ **테이블 및 차트 컴포넌트 작성 후 각 통계 데이터에 따라 컴포넌트 재사용**

- props를 이용하여 데이터 종류에 따라 테이블 및 차트 컴포넌트로 전달
- 전역상태에 테이블 및 차트 데이터 존재 유무에 따른 차트 및 테이블의 조건부 렌더링

✔️ **서브카테고리, 도메인, 채널, 유통 등 데이터 종류를 선택할 수 있는 버튼 컴포넌트**

- 활성화된 버튼의 내용과 대응하는 key 값 문자열을 `state`에 저장
- `state`에 저장된 문자열을 key 값으로 사용하여 전역상태에서 통계 데이터 추출
- 추출한 데이터에 따라 테이블 및 차트 화면 렌더링

