#Yolov5 버전별 학습

## 데이터셋 정보

### 데이터 구성
- **총 이미지 수**: 1,586장
- **클래스별 객체 수**:
  - gown_on (가운 착용): 3,273개
  - hairnet_on (모자 착용): 4,018개  
  - person (사람): 4,492개

### 데이터 분할
- **Training Set**: 1,189장 (75%)
- **Validation Set**: 237장 (15%)
- **Test Set**: 160장 (10%)

## 모델 설정

### 학습 파라미터
- **모델**: YOLOv5m (Medium)
- **Epochs**: 50
- **Batch Size**: 16
- **Image Size**: 640x640
- **GPU**: NVIDIA A100-SXM4-40GB

### 학습 결과
- **최종 mAP@0.5**: 97.8%
- **최종 mAP@0.5:0.95**: 69.0%
- **클래스별 성능**:
  - gown_on: Precision 95.9%, Recall 95.0%
  - hairnet_on: Precision 95.8%, Recall 91.2%
  - person: Precision 97.1%, Recall 97.8%

## 기술 스택

### 주요 라이브러리
- **Ultralytics**: YOLOv5 모델 구현
- **Roboflow**: 데이터셋 관리 및 전처리
- **PyTorch**: 딥러닝 프레임워크
- **OpenCV**: 컴퓨터 비전 처리
- **NumPy**: 수치 연산

### 개발 환경
- **Python**: 3.11.12
- **CUDA**: 12.4
- **Google Colab**: 클라우드 GPU 환경
