# <무인점포 이상행동 탐지 서비스>
# daboa
### 장려상
![image](https://github.com/user-attachments/assets/4bb72687-9c12-444b-a280-c4770bb1ddb2)

## 목차
| 순번 | 목차 항목 |
| :-: | :-: |
| 1 | [팀원 소개](#팀원-소개) |
| 2 | [프로젝트 기간](#프로젝트-기간) |
| 3 | [개요](#개요) |
| 4 | [배경](#배경) |
| 5 | [기대효과](#기대효과) |
| 6 | [시스템 설계](#시스템-설계) |
| 7 | [개발 과정](#개발-과정) |

## 팀원 소개

| _이름_ | 김준형 | 김가은 | 맹다혜 | 신유원 | 우민희 |
|:-----:|:----:|:-----:|:----:|:----:|:-----:|
| ___역할___ | BE, AI | FE | BE | AI | BE |
| ___Github___ | <a href="https://github.com/JHZLO"><img src="https://avatars.githubusercontent.com/u/105791673?v=4" width="64" height="64"></a> | <a href="https://github.com/ganyaaaaa"><img src="https://avatars.githubusercontent.com/u/141535219?v=4" width="64" height="64"></a> | <a href="https://github.com/Maengdahae"><img src="https://avatars.githubusercontent.com/u/164438476?v=4" width="64" height="64"></a> | <a href="https://github.com/youwon000218"><img src="https://avatars.githubusercontent.com/u/104317947?v=4" width="64" height="64"></a> | <a href="https://github.com/woominhee"><img src="https://avatars.githubusercontent.com/u/73922498?v=4" width="64" height="64"></a> |

## 프로젝트 기간
- 24.05 ~ 24.06

## 개요
![image](https://github.com/user-attachments/assets/ec5258d0-57cd-404d-bc5c-2eaab78ee566)

아이스크림 할인점 무인점포가 증가함에 따라 절도 사건 발생 건수가 급증하고 있다. 이에 따라 고객들의 이상행동에 대한 관리가 필요한 시점이다.

아이스크림 할인점 무인점포에서의 관리 대상 행동으로는 절도, 기물파손, 무단 취식 등이 있다.

이러한 문제를 해결하기 위해 인공지능 기술을 활용하여 CCTV 영상을 실시간으로 분석하고 이상 행동을 감지하여 기물파손, 폭행, 무단 취식과 같은 확실하게 판단 가능한 위반 행동 시에는 운영자에게 해당 사항을 알림과 동시에 자동적으로 ai 음성 송출하여 경고 메세지를 전달한다.

혹은 절도와 같은 중범죄의 행위에 해당하는 행동이 감지 된다면 이는 운영자의 선택으로 신고여부를 결정할 수 있도록 ai 음성 송출 대신 즉시 운영자에게 상황을 앱을 통해 알리고 신고여부를 결정하도록 하여 범죄를 예방한다.

## 배경
![image](https://github.com/user-attachments/assets/0b8c0ac9-2004-4b07-8953-9fbfad0a8162)
![image](https://github.com/user-attachments/assets/e865e517-a1f0-487d-83f3-fe9a5f96f96e)

무인점포의 도입은 인건비 절감을 목적으로 확산되고 있으나,이와 동시에 보안 취약성으로 인한 절도 손실이 증가하는 아이러니한 상황에 직면하고 있다.
또한 절도 발생 시, CCTV 영상 분석과 같은 후속 조치가 필요하며 이는 예상치 못한 추가 비용을 발생시킨다.
CCTV 영상을 검토하고, 필요한 경우 법적 조치를 취하는 과정에서 발생하는 시간과 비용은, 당초 인건비 절감을 통해 얻으려던 경제적 이득을 상쇄할 수 있다.

이는 무인점포 운영의 본질적인 목적에 역행하는 결과를 초래하며,
따라서 기업들은 무인 기술의 도입과 함께 첨단 보안 시스템에 대한 투자도 동시에 고려해야 할 필요성이 대두된다


## 기대효과

- **절도 예방** :
    
    절도를 실시간으로 감지하고 경고하여 절도를 예방할 수 있다.
    
- **비용 절감** :
    
    기존의 무인점포 운영자가 보안을 강화하는 방식은 단순히 cctv의 수를 늘려서 사각지대를 없애는 방향으로  범죄가 일어난 시점과 정황을 세밀하게 분석하였다.
    
    하지만 인공지능이 탑재된 cctv를 활용한다면 적은 cctv의 수로도 범죄를 탐지할 수 있다
    
    - 위에서 말한 사각지대란, 카드를 끝까지 꼽지 않는 행위와 같은 계산하는 척을 말함
- **시간 절약:**
    
    절도가 일어난 경우, 기존의 cctv로는 탐지를 할 수 없어 운영자가 범인을 찾기 위해서는 모든 시간대의 경우를 파악하고 분석해야하지만 인공지능 cctv를 활용한다면 절도 의심 알림이 일어난 시점을 위주로 범인을 찾을 수 있다.
    
## 시스템 설계
### 서비스 아키텍처
![image](https://github.com/user-attachments/assets/e2afb0e9-e8a9-4b30-95c3-1726019d5e22)
### 플로우 차트
![image](https://github.com/user-attachments/assets/dcaddcd9-7eed-43c0-92be-40e7ae56ebf2)

## 개발 과정

### 1. 데이터 선정
![image](https://github.com/user-attachments/assets/16748ff4-0ace-4d48-80a6-4a8024729df7)
![image](https://github.com/user-attachments/assets/786fa4e8-931b-454f-8093-72bd0fc50518)
- AI HUB의 이상행동/정상행동 데이터를 활용함
- 원본 데이터인 .mp4는 용량이 커서 다운, 학습하는 과정이 너무 오래걸림
- AI HUB에서 제공하는 라벨링된 데이터를 활용하여 바운딩 박스와 키 포인트 추출하여 학습을 진행
- 이상 행동의 시작 프레임과 끝 프레임 번호가 라벨링되어있으며 해당 프레임의 바운딩 박스와 34개의 키포인트들이 저장되어있

### 2. feature 추출 - yolo v8
![image](https://github.com/user-attachments/assets/94feffe6-4507-4a95-9e2b-4935d2d753c6)
- 프레임 단위로 사람을 탐지하고, 바운딩 박스와 키 포인트를 출력함
- 이를 통해 대용량의 입력 영상에서 피처를 추출하여 CSV 파일로 저장함으로써 용량 효율성을 크게 향상시킴
- 이러한 특징들을 LSTM모델의 입력으로 사용되어 시간적 특성을 모델링

### 3. 학습 모델 - LSTM AUTO ENCODER
![image](https://github.com/user-attachments/assets/474c3cdc-cffa-4286-9d55-a17c5c58c8a4)
![image](https://github.com/user-attachments/assets/f30f0762-2f76-4cfa-992b-0045216157ce)
- 비지도학습
- 입력된 정상 행동과 출력된 복원 행동 간의 차이를 줄이도록 학습합니다. 이상 행동 탐지에 있어 학습 데이터와 다른 이상 행동이 입력되면, 복원된 출력과 입력 간의 차이가 크게 발생합니다.
- 서비스 방향성에 맞춰 학습되지 않은 실제 이상 행동을 정상 행동으로 분류하는 치명적 오류를 피하기 위함
- 실시간 데이터 처리가 가능하며, 매장 내에서 발생하는 행동을 실시간으로 분석함





