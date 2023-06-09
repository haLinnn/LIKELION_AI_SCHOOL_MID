# 문화 지수를 통해 알아본 지역별 문화 격차
- 멋쟁이사자처럼 AI SCHOOL 8기 미드 프로젝트
- Member: AI SCHOOL 8기 7조 77움돌이
- Status: Complete
- Period: 23.02.16 ~ 23.02.26

## 01. 주제 선정 배경
지역별 문화 격차가 존재한다는 일반적인 생각과는 다르게 문화체육관광부의 보도자료나 단순 시설의 수만을 비교한 자료에서는 수도권과 비수도권 간의 차이가 없다는 결과가 나오기도 합니다. 이런 다양한 결과가 나오는 것이 대부분 인구를 기준으로 조사를 하거나 지역별 문화 다양성 변수를 배제한 결과라고 생각하였고, 버거지수에서 아이디어를 착안하여 문화 격차를 더 잘 표현할 저희만의 가치판단 기준을 세워 분석하였습니다.

문화 시설은 문화체육관광부에 따라 공연시설, 전시시설, 도서시설로 분류하였고 공연 시설에서는 영화관, 공연장을 선택하였고, 전시시설에서는 박물관, 미술관 그리고 도서시설에서는 도서관을 선택하여 분석했습니다.

## 02. 가설 수립
1. 인구수 대비 문화 시설의 개수는 수도권과 비수도권 지역간 큰 차이가 없을 것이다.
2. 실제 지역별 문화 시설의 규모, 운영 현황, 접근성 등을 반영하면 인구수 대비로 보더라도 지역간 격차가 존재할 것이다.
3. 문화 시설의 프로그램, 다양성을 비교하면 지역간 더 큰 격차가 존재할 것이다.

## 03. 데이터 출처
|시설|출처|데이터명|
|------|---|---|
|영화|영화진흥위원회|전국 극장 현황|
||영화관입장권통합전산망|전용상영관 현황|
||KOBIS|영화상영관별 상영내역|
|공연|KOPIS|공연정보 DB|
|박물관|문화빅데이터 플랫폼|박물관 시설 및 소장자료 통계 데이터|
||공공데이터포털|전국 박물관 미술관 정보 표준 데이터|
|미술관|문화빅데이터 플랫폼|국내 문화체육관광 분야 미술관 시설 및 현황 통계 데이터|
|도서관|국가도서관통계시스템|공공도서관 통계|

## 04. 분석 프로세스
1. 가설1 검증

 - 가설1: 인구수 대비 문화 시설의 개수는 수도권과 비수도권 지역간 큰 차이가 없을 것이다.
  
 <img src="https://user-images.githubusercontent.com/108817458/222506848-9ab93432-070f-4934-8918-f4cc4209ecf3.png" width="800" height="400"/> 

전체적으로 영화관 분포는 수도권에 집중되어 있었지만, 지역별 인구 10만명 당 스크린수를 보면 수도권과 비수도권 간에 차이가 없었다.


2. 지수 산정

   '폴란드와 우크라이나의 문화 기반시설의 영향성 평가 방법론' 논문 참고
  
- 문화인프라 지수 = 규모 * 가동률 * 접근성
- 문화다앙성 지수 = 프로그램 수 * 자료 수


  1) 영화관
     - 문화인프라 지수 = (좌석 수 * 상영 빈도 * 상영관 수) / (시도별 면적 * 시도별 인구수)
     - 문화다양성 지수 = 상영 편수(영화의 종류 * 상영관의 종류)
  
  2) 공연
     - 문화인프라 지수 = (규모 * 가동률) / (시도별 면적 * 시도별 인구수)
     - 문화다양성 지수 = 프로그램 수 * 자료 수
     
  3) 박물관•미술관•도서관
     - 문화인프라 지수 = (시설 면적 * 가동률) / (시도별 면적 * 시도별 인구수)
     - 문화다양성 지수 = 프로그램 수 * 자료 수


3. 가중치 적용

   문화체육관광부의 '2021년도 문화예술 행사 관람률 추이'를 근거로 각 문화시설에 가중치를 주어 전국 종합 문화지수를 산정
   
   - 영화: 76.3%
   - 공연: 17.1%
   - 박물관•미술관•도서관: 6.6%

## 05. 분석 결과
1. 전국 종합 문화 지수를 산정한 결과
  - 1등: 서울
  - 2등: 부산
  - 3등: 경기도
 
<p align="center"><img src="https://user-images.githubusercontent.com/108817458/222666750-30ab5760-6ec7-4c01-97c1-473bed8ec950.png" width="450" height="400"/></p>

2. 종합 문화 지수 등급

   종합 지수를 사분위수로 나누어 75-100%를 A, 50-75%를 B, 25-50%를 C, 나머지를 D로 기준을 세워 등급 산정

<p align="center"><img src="https://user-images.githubusercontent.com/108817458/222668086-50135621-53e2-4b9c-9c9f-4680167e8568.png" width="600" height="400"/></p>


위의 과정을 거쳐 분석한 결과 수도권 및 광역시 지역이 문화 지수가 높은 것으로 나타났고, 이를 통해 지역간 문화 격차가 있음을 검증하였습니다.
