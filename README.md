# 🐿 나의 작은 생태계(My Tiny Ecosystem)

---

## 개요(Summary)

환경빅데이터플랫폼 혁신서비스 아이디어 공모전 ( 2021.01.27 ~ 02.17 ) 

- 스마트폰 사용 시간이 점점 늘어가는 아이들을 위해 야외활동을 유발하는 서비스

  - 우리집 주변의 동물, 조류, 곤충 등의 서식지와 정보를 알려줌

-  팀원 : `허정훈`,  `구원혁`, `민성훈`, `진효정` </br></br>

Environmental Big Data Platform Innovation Service Idea Contest (2021.01.27 ~ 02.17)

- A service that induces outdoor activities for children whose smartphone usage time is increasing

  - It informs the habitat and information of animals, birds and insects around our house

- Team members:`Heo Jung-hoon`, `Gu Won-hyuk`, `Min Sung-hoon`, `Jin Hyo-jung`

---

  

## 데이터(Data)

* 데이터 출처 :  환경빅데이터플랫폼 [링크](https://www.bigdata-environment.kr/user/data_market/list.do)
* 50만개 정도의 곤충, 포유류, 조류 등의 동물 데이터가 있습니다.
* 그 종의 종명, 학명, 서식지 좌표 등의 데이터로 이루어져 있습니다.</br></br>

* Data source: Environmental Big Data Platform [Link](https://www.bigdata-environment.kr/user/data_market/list.do)
* There are 500,000 animal data such as insects, mammals and birds.
* It consists of data such as the species name, scientific name, and habitat coordinates of the species.


<img src = "https://user-images.githubusercontent.com/54921730/107643279-45290d80-6cb9-11eb-848e-4273c080134b.png" width = 1000 height = 150/>

<img src = "https://user-images.githubusercontent.com/54921730/107643337-5a05a100-6cb9-11eb-956d-3ea289a75d05.png" width = 1000 height = 260/>

---



## 좌표 변환(Coordinate Transformation)

* 국토지리정보원 표준 좌표계(중부원점 EPSG : 5186)인 좌표계를 GPS가 사용하는 좌표계인 EPSG : 4236로 변환 시켜 줌
  * PyProj 라이브러리 사용</br></br>
  
* Convert the coordinate system, which is the National Geographic Information Institute's standard coordinate system (Jungbu origin EPSG: 5186), into the coordinate system used by GPS, EPSG: 4236.
  * Use PyProj library

<img src = "https://user-images.githubusercontent.com/54921730/107644665-10b65100-6cbb-11eb-8c11-ffbc217ab57b.png" width = 1000 height = 500/>

---


## 유저 정보 입력(Enter User Information)

* 유저가 원하는 경위도와 반경 입력
    * 부산대학교와 3km 이내의 동물들을 찾아본다
      * haversine 라이브러리 사용</br></br>
      
* Enter the longitude and latitude and radius desired by the user
    * Search for animals within 3km of Pusan National University
      * Use the haversine library
      
<img src = "https://user-images.githubusercontent.com/54921730/107645442-047ec380-6cbc-11eb-8f68-f7d2f3b51dfc.png" width = 1000 height = 300/>

<img src = "https://user-images.githubusercontent.com/54921730/107645865-9dadda00-6cbc-11eb-8cd2-257f61eb2f28.png" width = 1000 height = 200/>

---

## 시각화

>   - 🕷(곤충/Insect) : 💛
>   - 🐍(양서파충류/Amphibians) : 💙 
> - 🐛(저서무척추동물/Benthos Invertebrate) : ❤️
> - 🦅(조류/Bird) : 💜
> - 🦝(포유류/Mammal) : 💚
>   - 원하는 마커를 클릭하면, 종과 이름, 사진 시각화
>   - Visualize species, names and photos by clicking on the desired marker
>     - 더 알아보기 클릭 시 해당동물의 위키피디아 정보 제공
>     - Click to learn more to provide Wikipedia information of the animal

<img src = "https://user-images.githubusercontent.com/51190752/107869190-9bbb6500-6ece-11eb-8441-f167805a69d1.jpg" width = 1000 height = 350/>

<img src = "https://user-images.githubusercontent.com/51190752/107869200-b8f03380-6ece-11eb-9380-816feabad8ea.jpg" width = 1000 height = 400/>

<img src = "https://user-images.githubusercontent.com/51190752/107868979-a7a62780-6ecc-11eb-9bc0-f22bba459586.jpg" width = 1000 height = 500/>
