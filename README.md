# 박민규 | Minkyu Park

서일대학교 IoT전자공학과 3학년 · 실제 환경에서 동작하는 AI 시스템을 만들고, 그것이 정말 동작하는지 실험으로 확인하는 일에 관심이 있습니다.

- **관심 분야**: 컴퓨터 비전, 멀티모달 AI (비전-언어 모델, LLM 응용)
- **연락처**: qkralsrb8973@gmail.com

## 대표 프로젝트

### [연구실 지능형 CCTV: 시간 흐름 판단 + 로컬 LLM·VLM](https://github.com/immmingyu/lab-cctv-ai)
`YOLOv8-Pose` `ByteTrack` `EXAONE 3.5` `Qwen3-VL` `FastAPI`

카메라 영상에서 낙상, 제한 구역 접근, 물건 이동을 시간 흐름으로 판단하고, 이벤트 기록을 로컬 LLM이 설명하는 관제 시스템입니다(캡스톤 디자인, 기획부터 구현·실험까지 단독 수행). 계산은 코드, 설명은 LLM으로 나눠 처음 보는 시험 질문에서 정답 6/12 → 10/12, 규칙이 놓친 자세는 조건부 VLM으로 재확인해 낙상 감지 9/15 → 13/15, 새 장소에서 실패하던 책 검출은 현장 파인튜닝으로 43/158 → 149/158로 개선했습니다. 개발용과 시험용 데이터를 나누고 설정을 결과 보기 전에 확정해 평가했습니다.

### [RC카 실시간 보행자 탐지: 경량 커스텀 CNN (Raspberry Pi 4)](https://github.com/immmingyu/rc-pedestrian-detection)
`PyTorch` `Custom CNN` `ONNX Runtime` `C++` `Raspberry Pi 4`

RPi4에서 실시간으로 동작하는 보행자 탐지 모델을 만든 3인 팀 프로젝트의 AI 파트입니다. 그리드 기반 커스텀 CNN에서 학습–추론 인코딩 불일치 버그를 찾아 고쳤고, 13회의 실험을 공통 기준으로 재평가해 비교했습니다. 파라미터 0.225M, 0.9MB 경량 모델로 RPi4 실측 13~15 FPS를 달성했습니다.

전체 시스템(카메라 → 탐지 → GPS 변환 → 위성지도 표시) 통합 저장소: [rc-pedestrian-mapping](https://github.com/immmingyu/rc-pedestrian-mapping)

## 기술 스택

| 분야 | 사용 경험 |
|---|---|
| 딥러닝 | PyTorch, Ultralytics YOLOv8, TensorFlow/Keras |
| 배포·추론 | ONNX Runtime (C++), TFLite, Raspberry Pi 4 |
| 백엔드·LLM·VLM | FastAPI, SQLite, Ollama (EXAONE 3.5, Qwen3-VL) |
| 기타 | OpenCV, Qt6, CMake, Git |
