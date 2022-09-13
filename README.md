# NanoChanllenge2
- Intelligence에 대해 알아보자!

## 개요

![image](https://user-images.githubusercontent.com/20871603/188385565-34413177-9a3a-4fe1-850c-2060a9870793.png)

## 서비스 방식

![image](https://user-images.githubusercontent.com/20871603/188385614-b4605a1b-1a88-483a-8bcb-7abec4641734.png)

## 인식 수신호

![image](https://user-images.githubusercontent.com/20871603/188385662-a3e6b331-ff8b-4043-9e40-5e926f198219.png)

## 기술 적용 방식

![image](https://user-images.githubusercontent.com/20871603/188385693-75e6df48-4c44-4340-9b73-5f2af4971d9a.png)

## 결과 및 목표

ML

- 현재 **동의 / 생각중 / 의견 보충 / 질문 / 반대** 의 경우 어느정도 학습이 되어 인식은 됨
- 하지만 데이터가 적어 학습 수준이 낮고, mlmodel의 학습에 고도화가 필요

App

- 학습한 모델을 앱에 올려 활용하는 것은 구현됨. (샘플 코드 변형)

![image](https://user-images.githubusercontent.com/20871603/188385735-3c8254d1-f893-40a4-8495-c26d56acf034.png)

## 이후 목표

ML

- background가 적음. 더 많은 background 확보 필요
- +) 더 많은 동작을 학습시키려고함
    - I see를 뜻하는 제스처 → 정지 동작이 아니므로 hand action classification 모델을 추가로 만들어야 함
    - 양 손을 동시에 사용하는 동작도 추가 예정

App

- 샘플 코드를 베이스로 일부 수정하는 것이 아니라 앱의 코드들을 직접 짤 예정
- 사용자의 정보를 넣어 누가 제스처를 취한 건지 나타낼 예정
- ‘방(회의실)’의 개념을 도입하여 함께 회의하는 유저들이 같은 방 안에서 리액션을 공유하도록 할 예정
- 하단의 테이블 뷰에 리액션이 기록되도록 할 예정
- 휘발되어도 괜찮은 리액션과 휘발되어선 안되는 리액션을 구분하여 기록할 예정
    - 동의 / 생각 중 → 휘발되어도 괜찮은 리액션
    - 반대 / 의견 보충 / 질문 → 휘발되어선 안되는 리액션 (상기되야 할 리액션)
        
        사용자의 확인 없이는 기록이 날아가서는 안 됨
        

## 참고 레퍼런스

[Apple Developer Documentation](https://developer.apple.com/documentation/createml/detecting_human_actions_in_a_live_video_feed)
