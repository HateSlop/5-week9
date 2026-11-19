# 9주차 과제

[공통 노트북](skeleton.ipynb)을 Colab에 업로드하고 Language·Vision·Speech 중 하나를 선택합니다.

## 제공 코드

- 기존 분할을 유지하고 없는 Train / Validation / Test 분할을 준비하는 함수
- 정답·예측 레이블로 Accuracy를 계산하는 함수
- 학습 전후 지표·예측 비교표
- LoRA 적용, 학습 실행, Adapter 저장 호출

## 완성할 TODO

모델·데이터 로딩, 전처리, 정답 열 추출, pipeline 추론과 예측 레이블 변환, LoRA 설정, Trainer 구성을 작성합니다. 생성형 Language 방식은 Prompt도 설계합니다.

같은 Test 데이터로 평가하고 최소 5개 출력을 비교합니다. 무작위 분할이 적절하지 않은 데이터는 화자·원본 등 그룹별로 분할합니다. 기본 Accuracy는 분류용이며 다른 태스크는 지표를 변경합니다.

## 참고 예시

[Vision 이미지 분류 모범 예시](result_vision_classification.ipynb)는 ViT-Small과 Beans를 사용한 LoRA 학습 코드, Colab 실행 출력과 결과 해석을 포함합니다. 노트북 구성과 결과 분석 방식을 참고하되, 모델·전처리·LoRA 대상 모듈과 추가 의존성은 선택한 태스크에 맞게 구현합니다.

## 제출

코드, 실행 출력, 설명과 분석을 모두 포함한 `.ipynb` 파일 하나를 제출합니다. Adapter, ZIP, CSV 등은 별도로 제출하지 않습니다. 설치된 라이브러리 버전, 학습 설정과 결과 분석을 노트북에 기록하고 실행 출력을 유지한 채 저장합니다.
