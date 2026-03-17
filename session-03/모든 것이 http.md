1. 전송 자원의 분류
 -> 텍스트와 바이너리 데이터

텍스트 기반 자원
  - 문서 구조 및 스타일: HTML(구조), CSS(디자인), JavaScript(동적 기능)
  - 데이터 교환 (API): JSON, XML. 현대 웹/앱 통신에서 데이터 교환의 표준으로 활용
  - 설정 및 기타: 웹 폰트 설정, 매니페스트 파일 등

바이너리 기반 자원
  - 멀티미디어: 이미지(JPEG, PNG, WebP, GIF), 동영상(MP4, WebM), 오디오
  - 문서 및 파일: PDF, 압축 파일(Zip), 실행 파일
  - 폰트: WOFF, WOFF2 등 웹 전용 폰트 파일

2. 핵심 보충 : 자원 식별 및 최적화
 -> 단순 전송 외에 클라이언트가 자원을 정확히 처리하기 위한 메커니즘
  - MIME Type (Content-Type): 서버는 응답 헤더에 Content-Type을 명시하여 브라우저가 자원(예: text/html, image/png, application/json)을 어떻게 해석할지 지시
  - 인코딩 및 압축: 전송 효율을 위해 gzip, br(Brotli) 등의 알고리즘으로 데이터를 압축하여 전송
  - 캐싱 (Cache-Control): 동일 자원의 재요청 시 서버 부하를 줄이기 위해 브라우저에 자원을 저장하도록 설정

3. 전송 및 처리 프로세스
  1. Request: 클라이언트가 URI를 통해 특정 자원을 요청
  2. Response: 서버가 해당 자원을 HTTP 응답 메시지의 바디에 담아 전송 (헤더에 데이터 정보 포함)
  3. Parsing & Rendering: * DOM/CSSOM 생성: 브라우저가 HTML과 CSS를 해석하여 구조화
    - Execution: JavaScript 엔진이 코드를 실행하여 동적 요소 적용
    - Painting: 해석된 데이터를 바탕으로 화면에 최종 픽셀을 출력