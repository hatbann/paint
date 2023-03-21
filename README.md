#  paint


# 📄 프로젝트 소개
 HTML, CSS, Javascript 실습을 위해 진행한 그림판 클론코딩사이트 입니다.

<br>

# ⌛ 제작 기간
2022년 4월 4일 ~ 2022년 4월 5일
<br>

# ⚙ 사용 기술 및 라이브러리
- `HTML / CSS`
- `Javascript`

<br>

# 🛠 주요 기능
<h3>1. 그림판 색 전체 칠하기</h3>

- 기본적으로 filling 변수를 false로하고, 만약 Fill 버튼을 클릭하면 true로 바꿔 모드를 전환합니다.
- canvas API의 fillRect 함수를 이용해 색칠합니다.

<h3>2. 그림 그리기</h3>

- Paint 버튼을 누르면 마우스로 그림을 그릴 수 있습니다.
- 마우스를 클릭할 시 painting변수가 true가 되고 마우스의 x, y 위치 값을 이벤트 객체의 offsetX와 offsetY를 통해 추척합니다.
- canvas API의 beginPath함수를 통해 그리기 시작하며 마우스를 떼면 painting 변수를 false로 바꿔 lineTo함수로 끝냅니다.

<h3>3. 선 두께 변명</h3>

- 그림판 하단에 위치한 슬라이더로 선 두께를 조절할 수 있습니다
- input type을 range로 하고, DOM을 선택해서 값이 변할 때마다 함수를 실행시켜 canvas의 lineWidth에 값을 저장해 두께를 바꿉니다.

<h3>4. 색상 변경</h3>

- 색을 선택하면 해당 색으로 화면 전체를 칠하거나 그림을 그릴 수 있습니다
- 기본적으로 canvas의 strokeStyle과 fillStyle을 지정하고 버튼을 클릭할 시 이벤트 객체의 backgroundColor를 가져와서 색을 설정합니다.

<h3>5. 저장 </h3>

- save버튼을 누르면 그린 사진을 저장할 수 있습니다
- canvas의 toDataURL를 통해 png로 바꾼 후 , document.createElement로 a태그를 만들고, 경로를 해당 png로 지정합니다.
- a태그의 download 메소드로 해당 이미지를 다운받습니다.


<br>

# 🖥 Site
https://hatbann.github.io/paint/
