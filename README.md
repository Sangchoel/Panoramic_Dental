# Panoramic_Dental 🦷
EfficientNet-B0을 백본으로 사용하는 UNet++ 기반  
**치과 파노라마 엑스레이 영상 자동 세그멘테이션** 프로젝트입니다.

> 📌 PyTorch 기반으로 구현되었으며, Google Colab에서 실험 및 학습을 수행했습니다.

---

## 📁 프로젝트 개요

- **목적**: 치아 파노라마 X-ray 이미지에서 충치 또는 관심 부위를 자동으로 분리(Segmentation)
- **모델 구조**: `UNet++ + EfficientNet-B0 (pretrained)`
- **데이터**: 사전 정제된 이미지/마스크 세트 사용
- **실행 환경**: Python, PyTorch, Google Colab

---

## ⚙️ 기술 스택

| 항목 | 내용 |
|------|------|
| 언어 | Python 3 |
| 프레임워크 | PyTorch |
| 모델 | UNet++ (with EfficientNet-b0 backbone) |
| 데이터 전처리 | torchvision, PIL |
| 시각화 | matplotlib |
| 평가 지표 | IoU, Dice, Accuracy, Sensitivity, Specificity |

---

## 🧪 주요 기능

- ✅ 이미지 및 마스크 데이터셋 전처리 (Grayscale 변환, Resize, Augmentation 등)
- ✅ DiceLoss 기반 커스텀 손실 함수
- ✅ IoU, Dice, Precision, Recall 등 정밀한 성능 평가
- ✅ 모델 저장 및 학습 로그(`log.txt`) 기록
- ✅ 예측 결과 시각화 및 GT 비교 (`matplotlib`)

---

## 🧰 실행 방법

> Colab 환경 기준

1. 필요한 라이브러리 설치  
!pip install segmentation_models_pytorch
# PyTorch와 TorchVision 설치 (Colab에 이미 설치된 경우가 많음)
!pip install torch torchvision

# OpenCV 설치
!pip install opencv-python-headless

# Matplotlib 설치
!pip install matplotlib

# Albumentations 설치 (선택 사항, 데이터 증강 시 유용)
!pip install albumentations


!pip install --upgrade sympy
# PyTorch 및 TorchVision 재설치
!pip install --upgrade torch torchvision

# sympy 최신 버전 설치
!pip install --upgrade sympy

!pip install tensorboard
     
