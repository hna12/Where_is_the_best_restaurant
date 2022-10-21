# 🍜Where to go for lunch in seongsu🍽

### 🌮Introduction
* SNS상의 수많은 맛집들.
* 하지만 그 중엔 광고글이 대다수이고
* 막상 가보면 그럭저럭한 곳이 꽤 많다.
* PURPOSE: 
  * 맛집평가와리뷰를 제공하는 사이트를 크롤링하여 **어느 위치**를 가야 맛있는 한끼식사를 할 가능성이 높은지를 조사하고 
  * 이를 함수화하여 위치만 입력하였을때 자동적으로 맛집을 list up 하여 csv파일로 만들어주는 코드 작성하는 것
### 🌮Methods and materials
* Methods: Python, BeautifulSoup library
* Materials: 네이버 지도, 포잉, 식신, 망고플레이트, 다이닝코드 </br>
(내가 맡은 사이트: 포잉)
### 🌮Result
TABLE1) 각 웹사이트에서 크롤링한 정보
</br>

정보 \ 웹사이트 | Poing | NAVER | Dining Code | Siksin | Mango Plate 
 ---|---|---|---|---|---|
상호 | O | O | O | O | O
전화번호 | O | O | O |  | 
주소 | O | O | O | O | O
리뷰수 | O | O | O |  | 
별점 | O |  | O | O | O
카테고리 | O | O | O | O | O
운영시간 |  | O |  |  |
홈페이지 |  | O |  |  |
메뉴 |  | O |  |  | 

</br>

1. 평점 있는 사이트에서의 결과. </br>

FIGURE1) POING의 맛집이 많은 도로 TOP5, POING의 평점이 높은 도로 TOP5 </br>
<img src = 'https://user-images.githubusercontent.com/61971952/197171469-74f9bb9d-4bf8-484e-af6b-6d18509d87b2.png' width = 40%, height = 40%>, <img src = 'https://user-images.githubusercontent.com/61971952/197171667-65c42de9-0af1-4ec1-838e-25a84831b413.png' width = 40%, height = 40%>

FIGURE2) MANGO의 맛집이 많은 도로 TOP5, MANGO의 평점이 높은 도로 TOP5 </br>
<img src = 'https://user-images.githubusercontent.com/61971952/197172170-ad0ddc23-4f07-49fa-bb8b-16bc5c326821.png' width = 40%, height = 40%>, <img src = 'https://user-images.githubusercontent.com/61971952/197172230-78e3b1f1-0648-4df9-83f2-2eb784d80b56.png' width = 40%, height = 40%>

FIGURE3) DININGCODE의 맛집이 많은 도로 TOP5, DININGCODE의 평점이 높은 도로 TOP5 </br>
<img src = 'https://user-images.githubusercontent.com/61971952/197172299-a2e2cb08-7833-4c4c-b962-00c974fd0f65.png' width = 40%, height = 40%>, <img src = 'https://user-images.githubusercontent.com/61971952/197172353-23549d0e-78e4-4cb0-8c26-01e48dcc0b65.png' width = 40%, height = 40%>

FIGURE4) SIKSIN의 맛집이 많은 도로 TOP5, SIKSIN의 평점이 높은 도로 TOP5 </br>
<img src = 'https://user-images.githubusercontent.com/61971952/197172395-f09d6fc6-741c-4c43-9838-2f851e42a5bd.png' width = 40%, height = 40%>, <img src = 'https://user-images.githubusercontent.com/61971952/197172448-096b27b2-0ca5-4ab7-bb9c-e6a794b8231e.png' width = 40%, height = 40%>

2. TABLE2) NAVER외 네개의 웹사이트를 종합하여 본 결과 TOP3 
    <br/>

    도로명 | 평점평균 | 가게수
    ---|---|---|
    연무장길 | 3.345 | 69
    연무장5가길 | 1.230 | 10
    아차산로 | 0.747 | 25
    </br>
3. 평점 없는 네이버의 결과. </br>

FIGURE5) NAVER지도 속 가게 수가 많은 도로 TOP5, NAVER지도 속 블로그 리뷰수가 많은 도로 TOP5 </br>
<img src = 'https://user-images.githubusercontent.com/61971952/197178521-552065d2-52cf-4f9c-bbbd-8778f1170a5a.png' widht = 250%, height = 250$>, <img src = 'https://user-images.githubusercontent.com/61971952/197179334-edade129-d3d2-4c5d-9188-a493a29f9222.png' widht = 250%, height = 250$>

### 🌮Discussion
1.  맛집의 개수가 많을수록 점수가 높을수록 그 도로를 가야 맛집을 갈 수 있는 확률이 높아진다.
2.  맛집 수, 리뷰 수, 평점위주로 집중해서 보았다.
3.  각 웹사이트 마다 갖고 있는 정보가 달랐다. 그 중 맛있는 정도를 평가할 수 있는 척도인 평점이 있는 사이트(NAVER 외4개의 사이트)와 없는 사이트(NAVER)로 나눠서 봄.
4.  또한 각 웹사이트마다 평점의 scale이 다양했다. Scale을 동일하게 주기위해 표준화(standardization)를 하였음. 
5.  모든 웹사이트의 결과를 종합해서 보았을 때 (TABLE2 & FIGURE5) **✨연무장길, 연무장5길, 아차산로✨**를 가면 맛있는 점심을 할 가능성이 많다는 결과가 도출할 수 있다.
