[CodeStates Project] 데이터를 활용한 출시 게임 설계
===

![01](https://github.com/Sanghoon-Oh-34/cs_project01/blob/main/2.%20Slides_images/01.jpg)

## 개요
* 코드스테이츠 AI 부트캠프에서 게임 데이터 분석을 주제로 진행한 프로젝트입니다.
* 주제: **다음 분기에 어떤 게임을 설계해야 할까?**
* 데이터셋: 1980 ~ 2020년 출시된 플랫폼별 게임&판매량 데이터 16,598건

## 내용
1. 문제인식  

 <img src='https://github.com/Sanghoon-Oh-34/cs_project01/blob/main/2.%20Slides_images/03.jpg' width='400px' height='300px'></img>
 <img src='https://github.com/Sanghoon-Oh-34/cs_project01/blob/main/2.%20Slides_images/04.jpg' width='400px' height='300px'></img>
* 다음 출시 게임을 결정하는 중요한 요소는 '매출'
* 플랫폼, 장르, 공급사에서 높은 매출액을 기록한 항목을 토대로 선정

<br>

2. 데이터 전처리  

<img src='https://github.com/Sanghoon-Oh-34/cs_project01/blob/main/2.%20Slides_images/06.jpg' width='400px' height='300px'></img>
<img src='https://github.com/Sanghoon-Oh-34/cs_project01/blob/main/2.%20Slides_images/07.jpg' width='400px' height='300px'></img>
* 결측치 처리: 전체의 2.3% 삭제, 데이터 분석에 큰 영향을 미치지 않는 소수의 데이터라 판단
* 지역별 매출액 화폐단위 상이하여 M(천만)으로 조정
* 이외 연도를 알기 어려운 데이터(ex. 1~10, 97, 98 등) 항목 삭제
<br>

3. 데이터 EDA

<img src='https://github.com/Sanghoon-Oh-34/cs_project01/blob/main/2.%20Slides_images/10.jpg' width='400px' height='300px'></img>
<img src='https://github.com/Sanghoon-Oh-34/cs_project01/blob/main/2.%20Slides_images/11.jpg' width='400px' height='300px'></img>
<img src='https://github.com/Sanghoon-Oh-34/cs_project01/blob/main/2.%20Slides_images/12.jpg' width='400px' height='300px'></img>
<img src='https://github.com/Sanghoon-Oh-34/cs_project01/blob/main/2.%20Slides_images/09.jpg' width='400px' height='300px'></img>
* 장르별 매출액 순위: 1위 액션 / 2위 스포츠 / 3위 슈팅
* 플랫폼별 매출액 순위: 1위 PS2 / 2위 X360 / 3위 PS3
* 공급사별 매출액 순위: 1위 닌텐도 / 2위 일렉트로닉아츠 / 3위 액티비전
<br>

4. 분석 및 결과  

<img src='https://github.com/Sanghoon-Oh-34/cs_project01/blob/main/2.%20Slides_images/17.jpg' width='400px' height='300px'></img>
<img src='https://github.com/Sanghoon-Oh-34/cs_project01/blob/main/2.%20Slides_images/18.jpg' width='400px' height='300px'></img>
<img src='https://github.com/Sanghoon-Oh-34/cs_project01/blob/main/2.%20Slides_images/19.jpg' width='400px' height='300px'></img>
<img src='https://github.com/Sanghoon-Oh-34/cs_project01/blob/main/2.%20Slides_images/20.jpg' width='400px' height='300px'></img>
* 기술의 발전, 경쟁사 출현 등 환경 변화에 따른 트렌드에 맞추어 최근 5년간 데이터 분석
* T-Test를 통해 항목별 1~2위 간 유의미한 차이가 있는 지 검증 진행
  - 플랫폼 1위 X360, 2위 PS3 차이 없음
  - 출고량 대비 매출액이 높은 플랫폼을 선택(X360 > PS3)
* 다음 분기 출시 게임 선정
  - 장르: 슈팅 / 플랫폼: X360 / 공급사: 액티비전
