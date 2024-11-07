# CP_MV
## 프로젝트 목적
AI모델인 Pose estimation을 활용하여 자세교정 프로그램을 구현합니다.<br/> 
## 개발환경
VScode, Linux(Ubuntu)
## 프로그램 로직
1. Pose Estimation 모델에서 관절 좌표를 얻습니다.<br/>
2. 좌표를 기반으로 세 점 사이의 각도 연산을 하여 관절의 각도를 구합니다.<br/>
3. 정답영상의 각 관절각도와 유저영상의 각 관절각도를 비교하여 유사도에 따른 점수를 부여합니다.<br/>
## 수행역할
관절각도 연산, 유저영상과 정답영상의 관절각도 유사도에 기반한 점수 산출 알고리즘을 구현했습니다.
## 시연영상
<img src="https://github.com/BrotherHwan/CP_MV/blob/main/image_video/cp_mv.gif" width=700 height=400> 


