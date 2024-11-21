# CP_MV
## 프로젝트 소개
Pose Estimation 모델을 활용하여, 정답영상과 사용자 영상을 비교합니다. 자세의 유사도에 따른 점수를 부여하여 사용자가 자세를 교정할 수 있도록 하는 프로그램입니다.<br/> 
## 구성인원
4명
## 기술 스택
![a](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white) ![b](https://img.shields.io/badge/Tensorflow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white) ![c](https://img.shields.io/badge/OpenCV-FF6F00?style=for-the-badge&logo=opencv&logoColor=white) ![d](https://img.shields.io/badge/Numpy-FF6F00?style=for-the-badge&logo=numpy&logoColor=white) ![e](https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white) ![e](https://img.shields.io/badge/Ubuntu-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white) 
## 역할
관절각도 연산, 유저영상과 정답영상의 관절각도 유사도에 기반한 점수 산출 알고리즘을 구현했습니다.
## 문제
1. 어떤 방식으로 자세를 교정할 수 있도록 할 것인가.
2. 프로그램 멈춤 현상 발생.
## 문제 해결 방안
1. 모델을 통해 신체 관절의 좌표값을 얻습니다. 좌표값을 이용하여 세 점 사이의 각도를 구합니다. 정답영상(숙련자의 영상)과 사용자의 관절각도를 비교하여 점수를 냅니다.
2. 멀티프로세스를 사용하고 프로세서간에 큐 통신을 이용합니다. 이를 통해 단일 프로세서의 부담을 줄입니다.
## 결과
자세 비교가 가능한 프로그램 구동
## 고찰
- 유저 영상에서 사람의 거리, 몸의 비율, 화면의 비율에 따라 관절각도가 영향을 받을 수 있고 자세비교의 정확성을 떨어뜨릴 수 있습니다.
- 프로그램이 너무 포괄적입니다. 춤, 스포츠, 재활 등 영상의 특성이 다른데 단순히 관절 각도 비교만 한다는 방식은 한계가 있었습니다. 차라리 한 가지 항목에 집중해서 더 퀄리티 높은 프로그램을 개발했었었어야 한다는 아쉬움이 있습니다.
- 단순 구현을 넘어서 성능개선, 성능측정에 신경을 썼어야 한다는 아쉬움이 있습니다.
## 시연영상
<img src="https://github.com/BrotherHwan/CP_MV/blob/main/image_video/cp_mv.gif" width=700 height=400> 
시연영상에 대한 설명<br/> 
1. 핸드제스쳐로 항목을 선택하고 실행합니다. <br/> 
2. 정답화면(큰 화면)을 보며 동작을 따라합니다. 유저화면은 우측상단에 위치합니다.<br/> 
3. 동작의 유사도에 따라 점수가 실시간으로 표시됩니다. <br/> 
4. 영상이 끝나면 점수가 낮은부분이 요약되고, 클릭하여 확인할 수 있습니다.<br/> 
