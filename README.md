# CP_MV
## 프로젝트 목적
AI모델인 Pose estimation을 활용하여 자세교정 프로그램을 구현합니다.<br/> 
## 기술 스택
![a](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white) ![b](https://img.shields.io/badge/Tensorflow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white) ![c](https://img.shields.io/badge/OpenCV-FF6F00?style=for-the-badge&logo=opencv&logoColor=white) ![d](https://img.shields.io/badge/Numpy-FF6F00?style=for-the-badge&logo=numpy&logoColor=white) ![e](https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white) ![e](https://img.shields.io/badge/Ubuntu-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white) 
## 프로그램 로직
1. Pose Estimation 모델에서 관절 좌표를 얻습니다.<br/>
2. 좌표를 기반으로 세 점 사이의 각도 연산을 하여 관절의 각도를 구합니다.<br/>
3. 정답영상의 각 관절각도와 유저영상의 각 관절각도를 비교하여 유사도에 따른 점수를 부여합니다.<br/>
## 수행역할
관절각도 연산, 유저영상과 정답영상의 관절각도 유사도에 기반한 점수 산출 알고리즘을 구현했습니다.
## 시연영상
<img src="https://github.com/BrotherHwan/CP_MV/blob/main/image_video/cp_mv.gif" width=700 height=400> 
시연영상에 대한 설명<br/> 
1. 핸드제스쳐로 항목을 선택하고 실행합니다. <br/> 
2. 정답화면(큰 화면)을 보며 동작을 따라합니다. 유저화면은 우측상단에 위치합니다.<br/> 
3. 동작의 유사도에 따라 점수가 실시간으로 표시됩니다. <br/> 
4. 영상이 끝나면 점수가 낮은부분이 요약되고, 클릭하여 확인할 수 있습니다.<br/> 
