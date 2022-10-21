# 🍜Where to go for lunch in seongsu🍽

### Introduction
* SNS상의 수많은 맛집들.
* 하지만 그 중엔 광고글이 대다수이고
* 막상 가보면 그럭저럭한 곳이 꽤 많다.
* PURPOSE: 
  * 맛집평가와리뷰를 제공하는 사이트를 크롤링하여 **어느 위치**를 가야 맛있는 한끼식사를 할 가능성이 높은지를 조사하고 
  * 이를 함수화하여 위치만 입력하였을때 자동적으로 맛집을 list up 하여 csv파일로 만들어주는 코드 작성하는 것
### Methods and materials
* Methods: Python, BeautifulSoup library
* Materials: 네이버 지도, 포잉, 식신, 망고플레이트, 다이닝코드 </br>
(내가 맡은 사이트: 포잉)
### Result
* 각 웹사이트에서 크롤링한 정보
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

1. 각 웹사이트 마다 갖고 있는 정보가 다름. 그 중 맛있는 정도를 평가할 수 있는 척도인 평점이 있는 사이트(NAVER 외.)와 없는 사이트(NAVER)로 나눠서 봄. </br>
2. 평점 있는 사이트에서의 결과. </br>
3. NAVER의 결과. </br>


### Discussion
