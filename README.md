# 🐿 나의 작은 생태계

---

## 개요

환경빅데이터플랫폼 혁신서비스 아이디어 공모전 ( 2021.01.27 ~ 02.17 ) 

- 스마트폰 사용 시간이 점점 늘어가는 아이들을 위해 야외활동을 유발하는 서비스

  - 우리집 주변의 동물, 조류, 곤충 등의 서식지와 정보를 알려줌

-  팀원 : `허정훈`,  `구원혁`, `민성훈`, `진효정`

---

## 데이터

* 데이터 출처 :  환경빅데이터플랫폼 [link](https://www.bigdata-environment.kr/user/data_market/list.do)
* 50만개 정도의 곤충, 포유류, 조류 등의 동물 데이터가 있습니다. [data](https://github.com/herjh0405/My_Tiny_Ecosystem/tree/master/data)
* 그 종의 종명, 학명, 서식지 좌표 등의 데이터로 이루어져 있습니다.

<img src = "https://user-images.githubusercontent.com/54921730/107643337-5a05a100-6cb9-11eb-956d-3ea289a75d05.png" width = 1000 max-width = 100% height = auto/>

---

## 좌표 변환

* 국토지리정보원 표준 좌표계(중부원점 EPSG : 5186)인 좌표계를 GPS가 사용하는 좌표계인 EPSG : 4236로 변환 시켜 줌
  * PyProj 라이브러리 사용
  

<img src = "https://user-images.githubusercontent.com/54921730/108377560-84220a80-7247-11eb-8d8f-01365061c030.png" width = 1000 max-width = 100% height = auto/>

---


## 유저 정보 입력

* 유저가 원하는 경위도와 반경 입력
    * 부산대학교와 3km 이내의 동물들을 찾아본다
      * haversine 라이브러리 사용
      

<img src = "https://user-images.githubusercontent.com/54921730/107645442-047ec380-6cbc-11eb-8f68-f7d2f3b51dfc.png" width = 1000 max-width = 100% height = auto/>

---

## 시각화

>   - 🕷(곤충) : 💛
>   - 🐍(양서파충류) : 💙 
>   - 🐛(저서무척추동물) : ❤️
>   - 🦅(조류) : 💜
>   - 🦝(포유류) : 💚
>   - 원하는 마커를 클릭하면, 종과 이름, 사진 시각화 
>     - 더 알아보기 클릭 시 해당동물의 위키피디아 정보 제공

<img src = "https://user-images.githubusercontent.com/51190752/107868979-a7a62780-6ecc-11eb-9bc0-f22bba459586.jpg" width = 1000 height = auto/>
