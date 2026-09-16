<a href="https://editor0124.tistory.com/" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/Tech_Blog-EB4747?style=for-the-badge&logo=tistory&logoColor=white"></a>
<a href="https://receipt-front.vercel.app/" target="_blank" rel="noopener noreferrer"><img src="https://img.shields.io/badge/Receipt_Service-000000?style=for-the-badge&logo=vercel&logoColor=white"></a>
<a href="mailto:banggujoong@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"></a>

</div>


## <span style="color: #EB4747;"> About Me</span>

* **Education**
  * 이화여자대학교 국제중국어교육학과 졸업
  * 대련외국어대학교 경제무역학과 졸업


## <span style="color: #e34c26;"> Tech Stack</span>

* **Language & Framework**: Java, Spring Boot, Python, FastAPI, React, Vue
* **AI & Messaging**: Google Gemini, Apache Kafka
* **Infrastructure**: Apache Airflow, Docker, Linux, AWS
* **Database & Cache**: PostgreSQL, MySQL, Oracle, Redis
* **Storage**: MinIO


## <span style="color: #2ea44f;"> Key Impacts (핵심 성과)</span>

* **데이터 수집 파이프라인**: 192만 건 조회 속도 <span style="color: #d73a49; font-weight: bold;">0.598초로 단축 (78% 향상)</span>, 서버 가동률 **100%**
* **회계 자동화 시스템**: 대용량 문서 처리를 통해 Gemini API <span style="color: #d73a49; font-weight: bold;">장애율 0%</span> 달성
* **이미지 처리 SaaS**: Redis 캐싱을 통해 이미지 조회 속도 <span style="color: #d73a49; font-weight: bold;">8ms 달성 (96% 단축)</span>


## <span style="color: #6f42c1;"> Major Projects</span>

### 01. 데이터 수집 파이프라인
* **기술 스택**: Python, FastAPI, Airflow, Selenium, MySQL, Redis, Docker
* **주요 성과**:
  * 브라우저 프로세스 관리 최적화로 크롤링 서버 다운 장애 원천 차단 (가동률 100%)
  * Keyset Pagination 도입으로 192만 건 조회 속도 78% 단축
  * 프록시 라우팅을 구축하여 WAF 차단 우회 및 수집 성공률 극대화


### 02. LLM 활용 영수증 이미지 분석 및 예산관리 시스템 *(개인 프로젝트)*
* **기술 스택**: Java, Spring Boot, Gemini, PostgreSQL, Redis, MinIO, Docker
* **서비스 링크**: [Live Demo](https://receipt-front.vercel.app/)
* **주요 성과**:
  * 슬라이딩 윈도우 방식으로 대용량 PDF 문서 분석 시 데이터 누락 방지
  * 지수 백오프 적용으로 API 호출 폭주(Rate Limit) 방어 및 장애율 0% 달성
  * Facade 패턴 적용으로 비즈니스 로직과 외부 API 호출부 분리


### 03. 이커머스 이미지 처리 모듈 (SaaS)
* **기술 스택**: Java, Spring Boot, Apache Kafka, Redis, PostgreSQL, MinIO, Docker
* **주요 성과**:
  * 이미지 바이너리를 Redis에 직접 캐싱하여 조회 속도를 8ms로 단축 (96% 향상)
  * Kafka 기반 비동기 처리를 도입해 스토리지 중복 I/O 80% 절감
  * 파일 매직 넘버 검증 로직을 추가하여 보안성 강화
