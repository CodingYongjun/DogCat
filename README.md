# 🐶독냥🐱# React Page
<br>
<div align="center">
  <img src="https://user-images.githubusercontent.com/108567709/226276847-3027617a-f4e8-4a6f-9e4a-923f4ce34838.jpg">
</div>

## 프로젝트 소개
<p>
  React로 구현한 강아지와 고양이 용품 쇼핑몰 사이트 입니다. 상세페이지와 장바구니 페이지 까지 구현 했습니다. 슬라이드 효과는 react-slick 라이브러리를 사용했으며 redux/toolkit을 사용해 장바구니 페이지를 관리할수있게 만들었습니다. 데이터는 json을 js에 담은것과 와 json파일을 만들어 관리하였습니다.
</p>

## 기술스택
<div align="center">
  <h3>📝SKill📖</h3>
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=React&logoColor=white" width="15%" height="50" />
  <img src="https://img.shields.io/badge/Sass-CC6699?style=flat-square&logo=Sass&logoColor=white" width="15%" height="50" />
  <img src="https://img.shields.io/badge/Javascript-F7DF1E?style=flat-square&logo=Javascript&logoColor=white" width="15%" height="50" />
  <img src="https://img.shields.io/badge/Redux-764ABC?style=flat-square&logo=Redux&logoColor=white" width="15%" height="50" />
</div>
<br>
<div align="center">
  <h3 align="center">🎮Tools🎮</h3>
  <img src="https://img.shields.io/badge/Visual%20Studio%20Code-007ACC?style=flat-square&logo=Visual%20Studio%20Code&logoColor=white" />
</div>

## 구현기능

<ol>
  <li>
    <h3>Routes,Route</h3>
    <br>
    <div align="center">
      <img src="https://user-images.githubusercontent.com/108567709/226276825-b45bc70e-8ef2-4f26-982a-2912ef2ae0d4.jpg">
    </div>
    <br>
    <ul>
      <li>  Routes,Route 를 이용해 주소에 맞게 컴퍼넌트가 바뀌게 해주었습니다.</li>
      <li>  hover시 filter:none 해주었고 transform:rotate() 값을 바꾸어서 동적이지 않게 간판이 움직이게끔 효과를 주었습니다.</li>
    </ul>
  </li>
  <li>
    <h3>react-slick , useState </h3>
    <br>
    <div align="center">
      <img src="https://user-images.githubusercontent.com/108567709/226276829-9a0a9f39-1ec6-4e44-ad50-ba970ab26bd7.jpg">
    </div>
    <br>
    <ul>
      <li>  첫번째 banner와 아래에 review 슬라이드는 react-slick 라이브러리를 사용해서 간단하게 만들어 주었습니다.</li>
      <li>  useState의 state값을 바꾸어주어 Tap을 구현해 주었으며 더보기 클릭시 새로운useState()가 생성이 되면서 그안에 json 형태로 만든 js파일을 담아주어 내용이 추가로 생성되게 해 주었다.</li>
    </ul>
  </li>
  <li>
    <h3>useState , useEffect , Outlet ,async , sort</h3>
    <br>
    <div align="center">
      <img src="https://user-images.githubusercontent.com/108567709/226276835-a2905bdb-e4a5-4069-8bc6-f7f50646476f.jpg">
    </div>
    <br>
    <ul>
      <li>  Tap을 구현해 주었으며 Outlet를 이용해 useNavigate 로 주소 변경시 아래의 컴퍼넌트가 바뀌게 끔 해주 었으며  useEffect를 통해서 서브메뉴를 클릭했을때도 Tap에따라 보여지는 제목의 값이 바뀌게끔 해 주었습니다.</li>
      <li>  async()함수를 이용해서 1번째 페이지와 2번째 페이지로 바뀔때 보여지는 json의 값이 바뀌게끔 해주었으며 이는 itemsPerPage = 4 이라는 함수를 만들어 json파일에서 4개씩만 보여지게끔 설정하였습니다. 그래서 총 8개의 json데이터가 4개씩 끊어져서 보여지게끔 설정해 주었습니다.</li>
      <li>  sort()함수를 사용해서 상품의 신상품 , 이름순 , 낮은 금액순 , 높은 금액순 으로 보여지는 기능을 구현했으며 여기서 신상품은 json데이터의 id값으로만 정렬해 주었습니다.</li>
    </ul>
  </li>
  <li>
    <h3>Nav</h3>
    <br>
    <div align="center">
      <img src="https://user-images.githubusercontent.com/108567709/226276837-fbdf5afb-fbf5-4939-8e64-155325125182.jpg" width="30%">
      <img src="https://user-images.githubusercontent.com/108567709/226276842-24cda695-3747-46f8-8dbc-3a155b1bf74d.jpg" width="30%">
    </div>
    <br>
    <ul>
      <li> 강아지와 고양이 용품의 서브페이지의 이름이 같아 사용자가 어느 파트의 sub 페이지를 보고있는지 구분을 주기위해서 nav의 배경사진과 색깔을 다르게 주었습니다.</li>
    </ul>
  </li>
  <li>
    <h3>Detail Page</h3>
    <br>
    <div align="center">
      <img src="https://user-images.githubusercontent.com/108567709/226276843-57d679c2-019c-4fc5-8853-2c815e610948.jpg">
    </div>
    <br>
    <ul>
      <li>  json 데이터의 id값을 useParams()가져와 split() 함수를 이용해 @ 로 나누어주고 나뉜 첫번째 값이 ~일때 어떤 json 데이터 파일을 가져와서 데이터값을 보여주게 했습니다.</li>
      <li>  클릭할때마다 숫자가 올라가게끔 useState()를 사용해 주었으며 총합 가격은 데이터의 price값*State 값을 주어 바뀌게 해 주었습니다.</li>
      <li>  redux를 이용해 장바구니 담기 클릭시 json 데이터를 push()함수로 가져와 따로 장바구니 페이지에 사용할수 있게 관리해 주었습니다. 이때  state.find()를 이용해 함수를 만들어준뒤 그함수를 if문을 걸어서 같을경우에는 제품을 추가하지 않고 그 제품의 count 값이 증가되게끔 해 주었습니다.</li>
    </ul>
  </li>
  <li>
    <h3>Cart Page</h3>
    <br>
    <div align="center">
      <img src="https://user-images.githubusercontent.com/108567709/226276845-22fe6167-9283-4aac-b1eb-f6a219c1ac12.jpg">
    </div>
    <br>
    <ul>
      <li>  redux에 담김 json데이터를 map()함수를 이용해 나타나게 해 주었습니다.</li>
      <li> + ,- 클릭시 redux의 count 값을 증가하고 감소하게 해주었고 여기서도 동일하게 count*price를 주어 금액이 변경되게 해주었으며 숫자가 1이하로는 떨어지지 않게 설정해 주었습니다. </li>
      <li>  왼쪽의 x 버튼 클릭시 action.payload로 전달된 값을 가진 데이터를 state에서 찾아 삭제되게 해주어 장바구니에서 상품이 삭제되게끔 해 주었습니다.</li>
      <li>  reduce()함수를 이용하요 초기값은 0으로 주었고 cur.count*price를 준 값을 acc와 + 해주어서 총 합의 값을 구해주었습니다.</li>
    </ul>
  </li>
 </ol>
