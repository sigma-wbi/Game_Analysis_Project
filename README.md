# 게임 판매량 통계 분석을 통한 후속 게임 설계 전략


## 프로젝트 소개
게임회사에 근무하는 데이터 분석가(DA)의 관점에서 '40년 간의 게임 판매량 통계'를 분석&시각화 하여 후속 게임 
설계에 대한 인사이트 도출

## 프로젝트 의의
* 방대한 양의 초기 데이터를 어떻게 정제&가공하여 분석에 용이한 데이터로 만들수 있는가
* 정제한 데이터를 다양한 파이썬 라이브러리를 통해 분석하고 시각화할 수 있는가
* 여러 결론이 나올수 있는 데이터를 가지고 합당하고 납득할만한 결론을 낼수 있는가

## Data
https://github.com/sigma-wbi/Section_1_Project/blob/main/vgames2.csv

## 📚Stack
![badge](https://img.shields.io/badge/Colab-F9AB00?style=flat-square&logo=googlecolab&logoColor=white)
![badge](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![badge](https://img.shields.io/badge/scikit-learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

## 분석 과정
https://github.com/sigma-wbi/Game_Analysis_Project/blob/main/Section_1_Project.ipynb

1. 데이터 정제
    - 16598개의 데이터를 .info() 메서드를 통해 데이터셋의 결측값이나 타입 확인
    - 중복값과 결측값 처리 : 중복값 삭제, 결측값은 삭제할 것인지 평균값등으로 매꿔서 사용할 것인지 선택 
    - 수학적 연산이 필요한 컬럼의 타입을 float로 변경
    - 12, 2012 등 같은 년도를 의미하는 값들을 통일
    - 분석에 필요하다고 생각되는 '전체 판매량' 컬럼을 계산하여 생성

2. 데이터 시각화&분석 : 게임 판매량 데이터셋을 보고 '다음 분기에 어떤 게임을 설계해야 하는가'에 대해 3가지 관점을 통해 시각화&분석
    - 지역에 따라 선호하는 게임 장르가 다른가
    - 연도별 게임의 트렌드가 있는가
    - 출고량이 높은 게임은 어떤 특징이 있는가

## 분석 결론
* 일본지역 게임 설계 전략과 그 외 지역(NA,EU,Other) 설계 전략을 따로 둔다.

* 일본지역은 Nintendo 계열 플렛폼에 충성도가 높고 롤플레잉 장르의 게임이 인기가 많다.
<br/>-> Nintendo 플랫폼을 활용한 Role-Palying 장르의 게임

* 그 외 지역(NA,EU,Other)은 PlayStation 플렛폼의 점유율이 가장 높고 액션, 스포츠 장르의 게임이 인기가 많다.

* 전체적으로 판매량이 급등한 2000년대 이후로 2006년 과 2009 년의 최고 장르가 스포츠인것으로 보아 4년마다 열리는 월드컵의 영향이 있을 것으로 보인다.

* 액션 장르는 확실히 1위 장르이지만 출고량 랭킹에서는 찾기 힘들었다. 이는 GTA 시리즈가 액션 장르의 대부분을 가지고 있었기 때문이다.

* 성공이 보장된 전작이 존재하는 시리즈 게임을 제작할시 GTA 시리즈와 유사한 엑션 장르 게임을 제작하는 것도 나쁘진 않지만 게임 하나를 제작하는 회사 입장에서는 판매량이 보다 고르게 분포되어 있고, 2위 장르였던 스포츠 장르를 선택하는 것이 더 좋다고 판단됨.

* 또한 2022년은 월드컵이 열리는 해 이므로 스포츠 장르를 택해야하는 이유에 좀 더 설득력을 준다고 생각한다.
<br/>-> NA,EU,Other 지역에는 PlayStation 기반의 스포츠 장르의 게임

<img width="80%" src="https://user-images.githubusercontent.com/81278907/232700899-10d90c04-458a-4f27-9a97-911a0d6812b5.png"/>

## 설명 영상
https://github.com/sigma-wbi/Game_Analysis_Project/blob/main/explanation_video.mp4



