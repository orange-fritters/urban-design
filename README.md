
![Title](https://capsule-render.vercel.app/api?type=transparent&fontColor=000000&text=Solving%20MCLP%20Using%20Graph%20Network%20and%20Genetic%20Algorithm%20&height=150&fontSize=30&desc=Proposal%20of%20the%20Location%20of%20New%20Elder%20Facilities%20in%20Gwanak&descAlignY=76&descAlign=50)  
---
<p>
<font size= "20">Resolving MCLP Using Walking Graph Network and Genetic Algorithm for the Proposal of Elder Facilities in Gwanak</font>
</p>

The final submission for **2022-F CEE Urban Design Final Project**

## Abstract

While Gwanak-gu has the fifth-highest percentage of elderly residents living alone in districts of Seoul, there are few elderly leisure facilities, therefore polarization is extreme. In this project, a walking **graph network** and **genetic algorithm** were used to offer new locations for elderly leisure facilities in Gwanak-gu. This study suggests a novel approach to calculate the score of the distributed locations using graph theories to solve **MCLP problem**.

## Data

This project used the data from [map.seoul.go.kr](map.seoul.go.kr)

<img src=images/data.jpeg width="640" height="360" />

- Distribution of Elder Populations
- Facility Supply Map
- Facility Demand Map


## Graph Embedding Using QGIS

This project used QGIS to obtain coordinates from the tif images and combined them together

<img src=./images/graph_embedding.jpeg width="640" height="360" />

<img src=./images/qgis.jpeg width="640" height="360" />


## Formula

Suggested Formula is below.

<p align="center">
  <img src=./images/formula.jpeg width="480" height="300" />
</p>

The objective function had to be created since there was no appropriate reference for the objective function that was to be used with the genetic algorithm. With a graph network, this formula was suitable as an objective function since it could perform complicated computations of the 4390X4390-sized matrix, result in quantitative values, and reflect the characteristics of the adjacent matrix. S is the importance score, L is the NX1 matrix of the location candidate obtained from the genetic algorithm's process, and D is the physical distance that cannot be represented on the node. These scores for each node are weighted to obtain the score of the location selection itself. One scalar-type score is produced on the graph by a matrix product.


## Result

The result is below.

<img src=./images/result.jpeg width="640" height="360" />



## Reference
```
[1] 김다솜, ＂서울 독거노인 35만명 넘어, 10명 중 3명 “고독사 우려" 「연합뉴스」, 2022년 5월 8일. 
[2] 정다은, 정광진, 유석연.(2021).서울시 지역생활서비스시설 불균등 분석.한국도시설계학회지 도시설계,22(2),59-78.
[3] 서울열린데이터광장(보건복지부 「노인복지시설 현황」), 2022.10.17
[4] 이태수, ＂노인의 생활반경은 ‘도보15분’ 경로당 자주, 오래 방문”  「연합뉴스」, 2017년 10월 12일
[5] “노인여가복지 인프라구축”, 서울시 정책지도, 2022년 10월 16일 접속, https://map.seoul.go.kr/spm/gly/policy/view.do?POLICY_CL_CODE=PLCAT20000&POLICY_NO=105
[6] 서울열린데이터광장(서울시 스마트도시담당관 「서울특별시 자치구별 장래인구추계」), 2022.10.17
[7] “Estimation of portfolio/SIP return using Monte Carlo-Python”, Medium, 2022년 10월 16일 접속, https://medium.com/@dstrader/monte-carlo-simulation-in-finance-python-part-2-13eb7bd89220
[8] “Genetic Algorith”, Papers with Code, 2022년 10월 16일 접속, https://paperswithcode.com/method/ga
[9] 조성아, 이건학. (2017). 공간 통계를 활용한 서울시 노년 인구 거주지와 노인 수요 시설 분포의 공간적 불일치 탐색. 한국도시지리학회지, 20(2), 99-112.
[10] 원종준, & 안건혁. (2010). 공공도서관 입지 및 시설특성이 이용활성화에 미치는 영향 연구: 서울시 공공도서관을 대상으로. 대한건축학회 논문집-계획계, 26(2), 79-86.
[11] 윤정미, & 이신훈. (2010). 효율성과 형평성을 고려한 공공시설 입지분석에 관한 연구-금산군 문화시설을 대상으로. 한국지리정보학회지, 13(2), 1-10.
[12] 마세인, & 김흥순. (2011). GIS 네트워크 분석을 활용한 노인복지시설의 접근성 연구: 인천시 내륙부를 중심으로. 국토연구, 61-75.
```



