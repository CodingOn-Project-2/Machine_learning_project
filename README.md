# AI 프로젝트

# 🍏 Food Intake Tracker & Calorie Calculator 🍽️

## 프로젝트 소개
**Food Intake Tracker & Calorie Calculator**는 사용자가 음식 섭취를 실시간으로 추적하고, 각 음식의 칼로리와 영양 성분을 계산하여 건강한 식습관을 유지하는 데 도움을 주는 시스템입니다. 이 프로젝트는 최신 AI 모델을 사용하여 실시간 영상 분석을 통해 음식 인식 및 칼로리 계산을 자동으로 처리합니다.

> **목표**: 음식 섭취를 추적하고 실시간으로 칼로리 정보를 제공하여 사용자가 자신의 식습관을 개선할 수 있도록 돕습니다.

## 주요 기능

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

## 🔗 링크

- [YOLOv5](https://github.com/ultralytics/yolov5)
- [USDA Food Database](https://fdc.nal.usda.gov/)

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


## 향후 계획
-----

## 기여 방법
프로젝트에 기여하고 싶다면, 다음 절차를 따라주세요:
1. 원격 저장소에서 새로운 브랜치를 생성합니다. (`git branch feature-branch`)
2. 생성한 브랜치로 이동합니다. (`git checkout feature-branch`)
3. 작업을 완료한 후, 해당 브랜치에 커밋과 푸시를 수행합니다.
4. 팀원들과 협의 후 `main` 브랜치에 병합합니다.

## 역할 분담
- [김소은](https://github.com/soeun1030) : -----
- [김성규](https://github.com/Seonggyu-art) : -----
- [김사무엘](https://github.com/koi154) : -----
- [송창우](https://github.com/songsungsang) : -----
- [조재원](https://github.com/jjw9728) : -----
