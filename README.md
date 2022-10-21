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

1. 각 웹사이트 마다 갖고 있는 정보가 다름. 그 중 맛있는 정도를 평가할 수 있는 척도인 평점이 있는 사이트(NAVER 외4개의 사이트)와 없는 사이트(NAVER)로 나눠서 봄. </br>
2. 평점 있는 사이트에서의 결과. </br>
FIGURE1) POING의 맛집이 많은 도로 TOP5 </br>
<img src = 'https://user-images.githubusercontent.com/61971952/197171469-74f9bb9d-4bf8-484e-af6b-6d18509d87b2.png' width = 40%, height = 40%>

FIGURE2) POING의 평점이 높은 도로 TOP5 </br>
<img src = 'https://user-images.githubusercontent.com/61971952/197171667-65c42de9-0af1-4ec1-838e-25a84831b413.png' width = 40%, height = 40%>

FIGURE3) MANGO의 맛집이 많은 도로 TOP5 </br>
<img src = 'https://user-images.githubusercontent.com/61971952/197172170-ad0ddc23-4f07-49fa-bb8b-16bc5c326821.png' width = 40%, height = 40%>

FIGURE4) MANGO의 평점이 높은 도로 TOP5 </br>
<img src = 'https://user-images.githubusercontent.com/61971952/197172230-78e3b1f1-0648-4df9-83f2-2eb784d80b56.png' width = 40%, height = 40%>

FIGURE5) DININGCODE의 맛집이 많은 도로 TOP5 </br>
<img src = 'https://user-images.githubusercontent.com/61971952/197172299-a2e2cb08-7833-4c4c-b962-00c974fd0f65.png' width = 40%, height = 40%>

FIGURE6) DININGCODE의 평점이 높은 도로 TOP5 </br>
<img src = 'https://user-images.githubusercontent.com/61971952/197172353-23549d0e-78e4-4cb0-8c26-01e48dcc0b65.png' width = 40%, height = 40%>

FIGURE7) SIKSIN의 맛집이 많은 도로 TOP5 </br>
<img src = 'https://user-images.githubusercontent.com/61971952/197172395-f09d6fc6-741c-4c43-9838-2f851e42a5bd.png' width = 40%, height = 40%>

FIGURE8) SIKSIN의 평점이 높은 도로 TOP5 </br>
<img src = 'https://user-images.githubusercontent.com/61971952/197172448-096b27b2-0ca5-4ab7-bb9c-e6a794b8231e.png' width = 40%, height = 40%>

맛집 등록이 많이 되어있는 도로일수록 맛있는 한 끼 식사를 할 가능성이 많다. 그렇기 때문에 맛집이 많이 분포하는 도로와 평점을 이용해 비교

3. NAVER의 결과. </br>

### 🌮Discussion
