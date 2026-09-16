<h2 align="center">👋 안녕하세요, 개발자 노민경입니다.</h2>
<p align="center"><b>비효율을 줄여 사용자 경험을 극대화하는 개발자</b>를 지향합니다.<br>새로운 기술을 배우고 적용하는 도전을 즐기며, 더 나은 결과물을 위해 끊임없이 고민하고 소통합니다.</p>

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/minjjings)
[![Tech Blog](https://img.shields.io/badge/Tech_Blog-EB4747?style=for-the-badge&logo=tistory&logoColor=white)](https://editor0124.tistory.com/)
[![Project](https://img.shields.io/badge/Receipt_Service-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://receipt-front.vercel.app/)

</div>


## <span style="color: #2b7489;"> About Me</span>

* **Experience & Background**
  * 이화여자대학교 외국어특수대학원 국제중국어교육학과 졸업
  * 대련외국어대학교 대외한어과 경제무역학과 졸업


## <span style="color: #e34c26;"> Tech Stack</span>

* **Language & Framework**: Java, Spring Boot, Spring Data JPA, Python, FastAPI ,React, Vue
* **AI & Messaging**: Google Vertex AI, Gemini, Apache Kafka
* **Data Pipeline & Infra**: Apache Airflow, Selenium, Chromium, Docker, Linux
* **Database & Cache**: PostgreSQL, MySQL, Oracle, Redis (Byte Caching)
* **Storage**: MinIO, AWS S3



## <span style="color: #2ea44f;"> Key Impacts (핵심 성과 요약)</span>

* **데이터 수집 파이프라인**: 192만 건 DB 조회 속도 <span style="color: #d73a49; font-weight: bold;">0.598초 단축 (78% 향상)</span>, 크롤링 서버 가동률 **100% 달성**, WAF IP 차단 **100% 우회**
* **LLM 기반 회계 자동화 시스템**: 대용량 PDF 문서 슬라이딩 윈도우 도입으로 문맥 손실 방지, 지수 백오프 적용을 통한 Gemini API <span style="color: #d73a49; font-weight: bold;">429 Rate Limit 장애율 0%</span> 달성
* **이커머스 이미지 처리 SaaS**: Redis 바이너리 직접 캐싱(Byte Caching)으로 이미지 조회 응답 속도 <span style="color: #d73a49; font-weight: bold;">8ms 달성 (96% 단축)</span>, 스토리지 I/O <span style="color: #d73a49; font-weight: bold;">80% 절감</span>


## <span style="color: #6f42c1;"> Major Projects</span>

### 01. 데이터 수집 및 고가용성 서빙 파이프라인

> **웹 데이터를 안정적으로 수집·스케줄링하고 대용량 DB로 조회 관리 시스템**

* **기술 스택**: Python, FastAPI, Apache Airflow, Chromium, Selenium, MySQL, Redis, Docker, GOST Proxy
* **주요 트러블슈팅 및 성과**:
  * **Chromium 프로세스 누적로 인한 리눅스 OOM Killer 방어**: Python Semaphore를 통한 동시 실행 제한 및 `try-finally` 블록 기반 브라우저 라이프사이클 관리로 **가동률 100%** 달성.
  * **192만 건 Deep Page 조회 레이턴시 최적화**: 기존 OFFSET 페이징의 Full Scan 한계를 극복하기 위해 하이브리드 Keyset Pagination 및 ASC 역방향 Seek 도입, 쿼리 응답 속도 **2.74s ➔ 0.598s (78% 단축)**.
  * **AWS 클라우드 IP 대역 차단 우회**: LocaltoNet 터널링과 GOST Hybrid Proxy 아키텍처를 결합한 5단계 라우팅을 구축하여 WAF 차단 **100% 우회 및 수집 성공률 극대화**.



### 02. LLM 활용 영수증 이미지 분석 및 예산관리 시스템 *(개인 프로젝트 / 회계 자동화 SaaS)*

> **수작업 중심의 회계 처리 한계를 극복하고, 메타 프롬프팅을 통해 회계 규정 및 영수증을 자동 파싱·정형화하는 AI 파이프라인**

* **기술 스택**: Java, Spring Boot, Spring Data JPA, Gemini, Google Vision API, PostgreSQL, Redis, MinIO, Docker
* **서비스 링크 & 레포지토리**:
  * **Live Demo (Service Site)**: [https://receipt-front.vercel.app/](https://receipt-front.vercel.app/)
  * **GitHub Repository**: [github.com/minjjings/receipt-front](https://github.com/minjjings/receipt-front)

* **주요 트러블슈팅 및 성과**:
  * **대용량 PDF 문서 토큰 한계 및 문맥 단절 극복**: 4,000자 Chunking + 200자 Overlap 기반의 슬라이딩 윈도우 파이프라인을 구축하여 대용량 규정 문서의 데이터 누락 0% 달성.
  * **API 호출 폭주(Rate Limit) 방어**: 지수 백오프(Exponential Backoff) 로직과 정규식 기반 JSON 정제 파이프라인을 적용하여 Gemini API 장애율 **0%** 달성.
  * **아키텍처 확장성 및 비용 최적화**: 서버 전처리 단에서 유효성을 사전 검증하는 Fail-Fast 패턴 적용으로 불필요한 API 과금을 차단하고, Facade 패턴을 도입하여 관심사 분리 및 유지보수성 극대화.



### 03. 이커머스 이미지 처리 모듈 (SaaS)

> **대용량 상품 이미지의 비동기 업로드 파이프라인을 구축하고 초고속으로 이미지를 직접 서빙하는 인프라 서비스**

* **기술 스택**: Java, Spring Boot, Spring Data JPA, Apache Kafka, Redis, PostgreSQL, MinIO, Docker
* **주요 트러블슈팅 및 성과**:
  * **Redis 바이너리 직접 캐싱을 통한 조회 성능 극대화**: URL 경로만 저장하던 방식에서 이미지 바이너리 데이터(Byte Array)를 직접 캐싱하는 구조로 변경하여, CDN/메모리 인스턴스 서빙 속도 **212ms ➔ 8ms (96% 단축)** 달성.
  * **Kafka 기반 비동기 메시징 도입**: 업로드와 리사이징/스토리지 저장을 비동기 이벤트 드라이븐 구조로 분리하여 동기식 서버 병목을 해소하고, 중복 I/O **80% 절감** 및 처리 속도 **46% 향상**.
  * **보안성 강화**: 단순 확장자 검사가 아닌 실제 파일 바이너리의 매직 넘버(Magic Number) 검증 로직을 도입하여 악성 파일 업로드 원천 차단.
