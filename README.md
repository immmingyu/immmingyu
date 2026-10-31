# 박민규 | Minkyu Park

서일대학교 IoT전자공학과 3 학년 · 실제 환경에서 동작하는 AI 시스템을 만들고, 그것이 정말 동작하는지 실험으로 확인하는 일에 관심이 있습니다.

- **관심 분야**: 컴퓨터 비전, 엣지 AI (경량화·임베디드 배포), LLM 응용 시스템
- **연락처**: qkralsrb8973@gmail.com

## 대표 프로젝트

### [RC카 실시간 보행자 탐지 (Raspberry Pi 4)](https://github.com/immmingyu/rc-pedestrian-detection)
`PyTorch` `YOLOv8` `ONNX Runtime` `C++` `Raspberry Pi 4`

RPi4에서 실시간으로 동작하는 보행자 탐지 모델을 만든 3인 팀 프로젝트의 AI 파트입니다. 제공받은 베이스 코드에서 학습–추론 인코딩 불일치 버그를 찾아 고쳤고, 13회의 실험을 공통 기준으로 재평가해 비교했습니다. 최종적으로 파라미터 0.225M, 0.9MB 모델로 RPi4 실측 13~15 FPS를 달성했습니다.

### 멀티모달 AI 기반 연구실 지능형 CCTV · 진행 중 (공개 예정)
`YOLOv8-Pose` `ByteTrack` `EXAONE 3.5` `FastAPI` `SQLite`

웹캠 영상에서 낙상·제한 구역 접근·물건 이동을 감지해 이벤트로 기록하고, LLM이 상황을 설명하고 질문에 답하는 관제 시스템입니다(캡스톤 디자인, 기획부터 구현·실험까지 단독 수행). 집계는 코드가, 설명은 LLM이 맡도록 역할을 나눠 환각을 줄였고, 지속 시간 기반 판단으로 숙이기 동작의 오경보를 0회로 줄였습니다.

## 기술 스택

| 분야 | 사용 경험 |
|---|---|
| 딥러닝 | PyTorch, Ultralytics YOLOv8, TensorFlow/Keras |
| 배포·추론 | ONNX Runtime (C++), TFLite, Raspberry Pi 4 |
| 백엔드·LLM | FastAPI, SQLite, Ollama (EXAONE 3.5) |
| 기타 | OpenCV, Qt6, CMake, Git |
