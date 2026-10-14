### 윤수용 · AI 서비스 백엔드 개발자

학습된 모델을 서비스로 연결하는 백엔드를 만듭니다.<br>
추론 서버, 비동기 파이프라인, 배포 자동화를 맡아 왔습니다.

[![Portfolio](https://img.shields.io/badge/Portfolio-yun--sooyong.github.io-284b63?style=flat-square)](https://yun-sooyong.github.io/)
[![Notion](https://img.shields.io/badge/Notion-이력·프로젝트_상세-000000?style=flat-square&logo=notion&logoColor=white)](https://app.notion.com/p/yun-sooyong/Portfolio-043bf3e871e1431ca97f3444bd5f3df2)
[![Blog](https://img.shields.io/badge/Blog-학습_노트-84a59d?style=flat-square)](https://yun-sooyong.github.io/blog/)
[![Email](https://img.shields.io/badge/ysyg22@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:ysyg22@gmail.com)

**주력 기술**<br>
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)

<sub>사용 경험: Celery · Redis · PostgreSQL · PyTorch · ONNX Runtime · Ollama · GCP(Cloud Run · Cloud Tasks · Cloud Storage) · GitHub Actions · Flutter</sub>

---

#### 대표 프로젝트

**[EMPATHO](https://github.com/medical-ai-group-3/empatho)** — 유방암 검진 경로 임상의사결정지원시스템 · 팀장 · 5인 · 2026.08–10 · 최종 프로젝트 우수상
- 판독 서버(FastAPI) 단독 개발: 판독 모델 4종을 한 창구로 묶고, 모든 실패를 HTTP 200 '기권'으로 반환
- MedSAM3 백본 1벌 공유 + 검사별 LoRA 교체: GPU 메모리 13,602 → 4,148 MiB, 결과는 비트 단위 동일
- LLM 소견문 서버: 수치는 코드가 문장화하고 모델은 문장만 엮음. 숫자가 바뀌면 코드가 만든 문장으로 대체
- Celery·Redis 판독 파이프라인(gpu·io 큐 분리), SSH 터널, 실패 시 자동 롤백하는 배포

**병리영상 분석 CDSS** — 유방암 병리영상 sTIL 분석 · 백엔드·GCP 인프라 단독 · 5인 · 2026.07
- Cloud Tasks + Cloud Run Job 비동기 추론 파이프라인, 작업 상태 5단계
- 업로드 실패 원인을 영상 151장 측정으로 찾음 (Cloud Run 32MiB 제한) → 서명 URL 직접 업로드로 전환
- FastAPI + ONNX Runtime 추론 서버, 설정 파일로 모델 추가, Workload Identity 기반 배포 자동화

그 외: 당뇨 재입원 위험 예측 대시보드(Django) · 의료진용 태블릿 앱(Flutter) — [포트폴리오](https://yun-sooyong.github.io/)에서 볼 수 있습니다.

#### 학습
- [dl-study](https://github.com/Yun-sooyong/dl-study) — 직접 만들며 배우는 딥러닝 · LLM · VLM (한국어 실습 코스)
- [블로그](https://yun-sooyong.github.io/blog/) — 학습 노트

<sub>건양대학교 융합IT · 정보처리기사 · 미래융합교육원 바이오메디컬 AI 개발 과정 (2026.03–10)</sub>
