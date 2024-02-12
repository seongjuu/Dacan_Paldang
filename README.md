# DACON 팔당댐 홍수 안전운영에 따른 한강 수위예측 AI 경진대회

## 🖥️ 배경
최근 기후변화로 인해 홍수 등의 자연재해가 지속적으로 발생함에 따라, 홍수 피해를 최소화하여 국민의 생명과 안전을 지키는 댐의 역할은 매우 중요해지고 있음.
팔당댐은 한국수력원자력(한수원)이 관리・운영 중인 댐으로, 서울 및 수도권의 홍수 방어에 있어 최후의 보루 역할을 하고 있음.
팔당댐의 홍수 안전운영에 따른 서울시내 한강 주요지점(잠수교 등)의 수위를 예측함으로써, 홍수재해로 인한 피해를 미연에 방지하고 최소화 할 수 있을 것으로 기대됨.

## ⏰ 기간
- 22.07.25~22.09.02
### 🧑‍🤝‍🧑 팀원
- 팀명 : 생각하는감자들
- 김성주, 성형훈, 이남선, 이동호, 조규원

## 📜 프로젝트 소개
- 보간법으로 데이터 결측치 처리
- Log 변환하여 왜도가 높은 데이터 분포 변환
- VAR 모델을 적용하기 위해 Granger causality, 다중공선성, 정상성 확인
- VAR(p) 모델의 최적 시차 p를 도출하기 위해 AIC 확인
- 모델 튜닝을 위해 학습데이터 기간, 스케일러, 변수 선택 방법 등 다양하게 시도
- Log변환 + VAR(232) 모델 + scaler 앙상블 모델 최종 선택

## 💽 사용데이터
- 대회 제공 데이터 : 팔당댐 현재수위, 유입량, 저수량, 공용량, 총 방류량, 강화대교 조위, 청담대교 유량, 잠수교 유량, 한강대교 유량, 행주대교 유량, 대곡교 강수량, 진관교 강수량, 송정동 강수량, 청담대교 수위, 잠수교 수위, 한강대교 수위, 행주대교 수위)
- 외부 데이터 : 한강 홍수 통제소-실시간 수문자료에서 청담대교, 잠수교, 한강대교, 행주대교의 test기간 데이터 수집, 해발표고 데이터 수집

## 🏆 결과
- 20등(Private 리더보드 상위 10%)
<img width="1194" alt="스크린샷 2024-02-12 오후 3 59 42" src="https://github.com/seongjuu/Paldang/assets/118152532/ae4ed3b4-6353-4424-ac43-9f1c8c44d957">
