# AI 프로젝트

# 🍏 Food Intake Tracker & Calorie Calculator 🍽️

## 프로젝트 소개
**Food Intake Tracker & Calorie Calculator**는 사용자가 음식 섭취를 실시간으로 추적하고, 각 음식의 칼로리와 영양 성분을 계산하여 건강한 식습관을 유지하는 데 도움을 주는 시스템입니다. 이 프로젝트는 최신 AI 모델을 사용하여 실시간 영상 분석을 통해 음식 인식 및 칼로리 계산을 자동으로 처리합니다.

> **목표**: 음식 섭취를 추적하고 실시간으로 칼로리 정보를 제공하여 사용자가 자신의 식습관을 개선할 수 있도록 돕습니다.

## ⚡ 주요 기능

### 🍔 **음식 인식**
- 실시간 카메라 영상을 통해 음식 객체를 인식합니다.
- YOLOv5와 같은 객체 탐지 모델을 사용하여 음식 종류를 정확하게 식별합니다.

### 🍎 **칼로리 계산**
- 각 음식에 대한 칼로리와 영양 정보를 계산하여 사용자에게 제공합니다.
- **USDA Food Database** 또는 **Open Food Facts**를 기반으로 한 음식 칼로리 데이터베이스 사용.

### 🧑‍⚕️ **영양 성분 추적**
- 각 음식의 영양 성분을 추적하여 사용자가 섭취한 칼로리 외에도 탄수화물, 단백질, 지방 등의 영양 상태를 관리할 수 있도록 합니다.

### 🛎️ **알림 시스템**
- 사용자가 음식 섭취를 할 때마다 실시간 알림을 통해 섭취 칼로리를 알려줍니다.
- 예: "Apple detected! 95 calories" 또는 "Total Calories: 285 calories".

## 💻 시스템 요구 사항

![Python Version](https://img.shields.io/badge/Python-3.8%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-v1.8-red)
![YOLOv5](https://img.shields.io/badge/YOLOv5-v5.0-green)

- Python 3.x 이상
- OpenCV
- PyTorch
- YOLOv5 (객체 탐지 모델)
- Plyer (알림 기능)

## 📸 데모

**음식 인식 및 칼로리 계산**의 예시 화면

![Food Intake Demo](https://via.placeholder.com/800x400.png?text=Food+Intake+Demo)  
_음식 인식 및 칼로리 계산의 예시 화면_

---

## 📈 발전 방향

- **다양한 음식 데이터 추가**: 더 많은 음식 종류와 칼로리 정보를 데이터베이스에 추가하여 인식 범위를 확장.
- **모바일 앱 연동**: 모바일 앱에서 실시간 음식 추적 및 칼로리 계산 기능을 제공하여 언제 어디서나 사용 가능.
- **AI 학습 개선**: 음식 인식 정확도를 높이기 위해 더 많은 데이터를 사용하여 AI 모델을 지속적으로 학습시킵니다.

---

## 🚧 문제 해결과 도전 과제

### 1. 객체 인식 정확도 향상

처음에는 YOLOv5의 사전 학습된 모델을 사용했지만, 음식 인식 정확도가 낮았습니다. 이를 개선하기 위해 **데이터셋을 커스터마이즈**하고 **Fine-tuning**을 진행하여 모델의 정확도를 높였습니다.

### 2. 실시간 속도 최적화

실시간 영상에서 음식 객체를 인식하는 과정에서 지연 시간이 길어졌습니다. 이를 해결하기 위해 **프레임 크기를 줄이고** 모델 추론 속도를 최적화하였으며, **멀티스레딩**을 사용하여 성능을 개선했습니다.

### 3. 칼로리 데이터 출처

음식 칼로리를 실시간으로 계산하기 위해 **Open Food Facts API**와 **USDA Food Database**를 사용했으며, 이들 API의 데이터 형식 차이를 해결하기 위해 데이터 전처리를 진행했습니다.

---

## ❓ 자주 묻는 질문 (FAQ)

### Q: 프로그램이 카메라를 인식하지 않아요.
A: 카메라가 제대로 연결되지 않았을 수 있습니다. 다른 USB 포트에 카메라를 연결해 보세요. 또한, OpenCV가 카메라를 제대로 인식할 수 있도록 필요한 드라이버가 설치되어 있는지 확인하세요.

### Q: 음식 인식이 정확하지 않아요.
A: 모델의 정확도를 높이기 위해 **Fine-tuning**이 필요할 수 있습니다. 데이터셋을 추가하거나 **YOLO 모델을 재학습**하여 개선할 수 있습니다.

### Q: 알림이 제대로 오지 않아요.
A: `plyer` 라이브러리가 알림을 정상적으로 표시할 수 있도록 환경에 맞는 설정을 해주세요. 예를 들어, Windows에서는 `pywin32`가 필요할 수 있습니다.

---

## 🔗 링크

- [YOLOv5](https://github.com/ultralytics/yolov5)
- [USDA Food Database](https://fdc.nal.usda.gov/)

---

## 🍽️ 음식 데이터베이스 비교

| 데이터베이스 | 출처                    | 제공하는 정보        |
|--------------|-------------------------|----------------------|
| USDA         | [USDA Food Database](https://fdc.nal.usda.gov/) | 음식 칼로리, 영양 성분 |
| Open Food Facts | [Open Food Facts API](https://world.openfoodfacts.org/) | 칼로리, 성분, 라벨 정보 |

---

## 📝 Contributing

이 프로젝트에 기여하고 싶다면 다음 절차를 따르세요:

1. **저장소를 Fork 합니다.**
2. **새로운 기능을 추가하거나 버그를 수정합니다.**
3. **Pull Request를 생성하여 기여 사항을 제출합니다.**

### 컨트리뷰팅 절차

1. **이슈 리포팅**: 발견한 버그나 개선 사항을 [이슈](https://github.com/----/----/issues)로 등록해 주세요.
2. **새로운 기능 추가**: 새로운 기능을 추가할 때는 각 기능에 대한 문서도 함께 작성해 주세요.
3. **코드 스타일**: 코딩 스타일 가이드에 맞춰 작성해 주세요. Python PEP 8 스타일을 따르세요.
4. **테스트 작성**: 기능을 추가한 후에는 반드시 해당 기능에 대한 테스트 코드를 작성해 주세요.


## 🚧 향후 계획
-----

## 📈 기여 방법
프로젝트에 기여하고 싶다면, 다음 절차를 따라주세요:
1. 원격 저장소에서 새로운 브랜치를 생성합니다. (`git branch feature-branch`)
2. 생성한 브랜치로 이동합니다. (`git checkout feature-branch`)
3. 작업을 완료한 후, 해당 브랜치에 커밋과 푸시를 수행합니다.
4. 팀원들과 협의 후 `main` 브랜치에 병합합니다.

## 📂 프로젝트 구조

프로젝트의 기본 폴더 구조는 다음과 같습니다:

```plaintext
food-intake-tracker/
│
├── food_intake_tracker.py        # 메인 실행 파일
├── requirements.txt              # 필요한 라이브러리 목록
├── README.md                    # 프로젝트 설명 파일
├── models/                       # YOLOv5 모델 파일
│   └── yolov5s.pt                # YOLOv5 사전 학습된 모델
└── data/                         # 음식 데이터 파일
    └── food_data.json            # 음식 칼로리 및 영양 정보
```

---
 
## 🧑‍⚕️ 역할 분담

- 🍏 [김소은](https://github.com/soeun1030) : -----
- 🍎 [김성규](https://github.com/Seonggyu-art) : -----
- 🍊 [김사무엘](https://github.com/koi154) : -----
- 🍉 [송창우](https://github.com/songsungsang) : -----
- 🍓 [조재원](https://github.com/jjw9728) : -----

---

## 🔗 기여자 링크

- 🔗 [김소은 GitHub](https://github.com/soeun1030)
- 🔗 [김성규 GitHub](https://github.com/Seonggyu-art)
- 🔗 [김사무엘 GitHub](https://github.com/koi154)
- 🔗 [송창우 GitHub](https://github.com/songsungsang)
- 🔗 [조재원 GitHub](https://github.com/jjw9728)

