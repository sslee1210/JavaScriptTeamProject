# 🍅 팀프로젝트
## 🎯 프로젝트 목표

#### 1. 다양한 이미지를 활용하여 디자인을 구현할 수 있다.
#### 2. 팀원들 간의 활발한 소통으로 원활한 의견 교환이 이루어 질 수 있게 한다.
#### 3. 홈페이지에 필요한 기능들을 파악한 후 필요한 능력을 학습하여 개인의 능력을 증진시킨다.
#### 4. GITHUB ORGANIGATION을 통해 파일을 공유하여 GITHUB 활용 능력을 기른다.
#### 5. 정해진 시간 내에 홈페이지를 최대한 흡사하게 구현한다.
---
### ⏱ 개발 기간: 2023.10.25 ~ 2023.11.12

---

## 🛠 사용 기술 및 도구
#### **프로젝트 관리:** `Github` `Figma` `Notion` `PowerPoint`
  
#### **사용기술:** `JavaScript` `HTML5` `CSS3`

---
   
## 👨‍👩‍👧‍👦 팀원 및 역할 담당
#### **이성수:** sub3 페이지 구현, Header와 Footer 영역 구현, 전체 파일 관리, 요구분석과 구조분석 작성, PPT 제작

#### **성영은:** sub2 페이지 구현, GITHUB 관리, 퍼블리싱 가이드 작성, 프로젝트 보고서 작성

#### **이현범:**  sub1 페이지 구현, PPT 제작

#### **허수인:** main(index) 페이지 구현, PPT 제작, PPT 발표

---

## 📍 작업 순서
#### 1. 레퍼런스 사이트 조사, 선별
#### 2. 각 페이지 별 업무 분담
#### 3. 퍼블리싱 가이드 작성 (common 작성)
#### 4. 디렉토리 구조 설정
#### 5. pc버전, 모바일 버전 홈페이지 마크업
#### 6. 각자 맡은 페이지 구현 작업 (html → css → js 순서)
#### 7. 각자 완성된 페이지 연결
#### 8. 연결 후 일어나는 오류와 위치값 수정
#### 9. 작업 마무리 및 발표 준비

---
  
## ✏ 퍼블리싱 가이드
<details>
<summary>공통사항</summary>
  
 - 선택자에 사용되는 띄어쓰기는 언더바(_)로 통일. 단 js의 경우 카멜 표기법을 이용한다.

```
// 언더바 사용
<div class = "course_box">
```

```
// 카멜 표기법 사용
"courseBox"
```

 - 들여쓰기는 space 2를 기준으로 한다.
 - W3C 유효성 검사를 이용해 오류를 확인하여 작업한다.
 - 해상도 기준은 PC = 1200px로 정하고 모바일 우선으로 작업한다.
 - 문서에서 각 영역은 각주와 한 줄 띄어쓰기를 이용해 정리한다.
```
</section>
<!-- section -->
<section> ...
```
     
```
...
margin: 2vw;
}
/* section */
.section {...
```
 - 파일에 사용되는 띄어쓰기는 하이픈(-)으로 통일하고 알맞은 폴더에 정리한다.
</details>

<details>
<summary>HTML</summary>

#### 기본 작성방법
- 페이지 로고 작업 시 , 기본적으로 img 태그를 사용하나, 필요에 따라 backgroundimage로 처리한다.
- 페이지 내 각 영역은 역할에 따라 head, section, footer 태그를 사용한다.
- 선택자 명은 페이지 내용을 바탕으로 의미 있고 알아보기 쉬운 이름을 사용한다.
 
```
<div class = "course">
<div class = "course_box">
```

#### 연결방법
- 외부문서는 <head> 영역 <title>바로 밑에 <link>로 작성한다.
- <reset>, <common>, <favicon>, <style>, <js> 순서로 작성한다.
- 미디어 쿼리 기준 선언은 스타일 시트의 <link> 태그 안에 작성한다.

```
<link rel = "stylesheet" href = "./style-pc.css" media = "(width >= 1200px)">
```

- 플러그인의 경우 바디 영역 제일 마지막에 삽입하여 작업한다.
- id 속성자의 경우 꼭 필요한 경우에만 사용하고 불필요한 경우에서의 사용을 지양한다.
- favicon의 경우 assets 폴더의 png 파일을 link로 걸어서 사용한다.
 </details>

<details>
<summary>CSS</summary>

- 폰트와 아이콘 등 중복되는 소스는 assets 폴더를 이용하여 공유한다.
- 컬러는 #컬러코드와 소문자를 이용하여 작성.

```
#FF5C9B, rgb(225,92,155) ... - X
#ff5c9b - O
```

- 사이즈 값은 상황에 따라 rem, vw를 혼용하여 사용한다.
- 값이 “0”인 경우에는 단위를 생략한다.
- 선택자 작성 시 하위 선택자 작성 방식을 사용한다.
</details> 

<details>
<summary>JAVA SCRIPT</summary>

- 기본적으로 큰 따옴표(””)를 사용하고 필요 시에만 백틱(``)을 사용한다.
- const를 사용하여 모든 지역 변수를 선언. 변수를 다시 할당해야 할 경우에만 let을 사용하고 var의 사용은 지양한다.
- 선언 시 이름은 html에서 사용한 선택자 명을 바탕으로 카멜 표기법으로 작성한다.

```
const kitTitle = document.querySelector(".kit_title");
```

- 필요한 경우 코드 옆에 주석을 달아 현재 코드가 어떤 기능을 하고 있는지 설명한다.
</details>
---
   
## 📁 디렉토리 구조 분석
    
<img src="https://github.com/sslee1210/JavaScriptTeamProject/assets/142865231/b0fce6f0-2117-42c9-9e73-1ad8fe7e746a.png"  width="550" height="auto"/>
   
---

## 📃 요구 분석

<img src="https://github.com/sslee1210/JavaScriptTeamProject/assets/142865231/0fdd11c2-c5c2-4d37-8d49-007efd0c3053.png"  width="600" height="auto"/>

---  

# 🎈 프로젝트 회고


## 🗝 문제 및 해결

### 상황 1
  - #### 문제 발생:
      햄버거버튼 드롭다운 메뉴 구현이 잘 안됨.

  - #### 해결 방안:
      span을 이용해 바 모양을 잡아주고 transform: translate(0, -50%) rotate(90deg)로 마우스를 누르면 x모양으로 바뀌게 함.

```
<!-- 햄버거 아이콘 -->
<input type="checkbox" id="icon" />
  <label for="icon">
    <span></span>
    <span></span>
    <span></span>
  </label>
```

```
#icon + label {
  display: block;
  width: 30px;
  height: 20px;
  cursor: pointer;
  position: relative;
  bottom: 5vw;
}

#icon + label > span {
  position: absolute;
  display: block;
  width: 100%;
  height: 3px;
  border-radius: 30px;
  background: #000;
  transition: all 0.35s;
  z-index: 2;
  left: 85vw;
}

#icon + label > span:nth-child(1) {
  top: 0;
}

#icon + label > span:nth-child(2) {
  top: 50%;
  transform: translateY(-50%);
}

#icon + label > span:nth-child(3) {
  bottom: 0;
}

#icon:checked + label > span:nth-child(1) {
  top: 50%;
  transform: translateY(-50%) rotate(45deg);
}

#icon:checked + label > span:nth-child(2) {
  opacity: 0;
}

#icon:checked + label > span:nth-child(3) {
  bottom: 50%;
  transform: translateY(50%) rotate(-45deg);
}

#icon + label + #wrap {
  position: fixed;
  top: 0;
  right: -300%;
  width: 100vw;
  height: 100%;
  background: #f5f5f5;
  color: #000000;
  z-index: 1;
  transition: right 0.3s ease; /* 애니메이션 효과를 주기 위한 transition 속성 */
```

### 상황 2
  - #### 문제 발생:
      모바일 버전에서 메뉴 버튼을 누르면 서브 메뉴가 오른쪽에서 왼쪽으로 스윽 나타나는걸 구현하기 힘들었음.
      
  - #### 해결 방안:
      자바스크립트로 위치를 right:-300%로 브라우저 바깥에 있다가 메뉴버튼을 누르면 right:0으로 만들었더니 해결됨.
```
// 헤더 메뉴바
window.onload = function () {
  document.addEventListener("DOMContentLoaded", function () {
    const menuIcon = document.getElementById("menu-icon");
    const wrap = document.getElementById("wrap");

    menuIcon.addEventListener("click", function () {
      // 햄버거 바를 클릭할 때마다 헤더가 나타났다가 사라졌다가 함
      if (wrap.style.right === "0px") {
        wrap.style.right = "-300%";
      } else {
        wrap.style.right = "0";
      }
    });
  });
};
```    

### 상황 3
  - #### 문제 발생:
      스크롤을 끝까지 내렸을 때 화살표가 오른쪽 하단에 position:absolute로 고정되어 있다가 스크롤을 올리면 position:fixed로 바뀌며 따라 올라가야 되지만 absolute에서 fixed로 바뀌지 않음.

  - #### 해결 방안:
      해결법을 찾지못해 스크롤을 끝까지 내리면 버튼이 사라졌다가 다시 스크롤을 올리면 브라우저 오른쪽 맨 하단에서 따라 올라가는 기능밖에 구현하지 못함 추후에 더 공부할 예정.

```
document.addEventListener("DOMContentLoaded", function () {
  var contentSection = document.getElementById("content");
  var backButton = document.querySelector(".btn_top"); // "btn_top"이라는 클래스를 가진 요소를 backButton 변수에 저장합니다.

// 스크롤 위치에 따라 '위로 가기' 버튼의 표시 여부를 조정하는 함수입니다.
  function toggleBackButton() {

    // 스크롤이 "content" 요소의 시작 위치를 넘어갔다면
    if (window.scrollY > contentSection.offsetTop) {

      // '위로 가기' 버튼을 보이게 합니다.
      backButton.classList.add("show");
    } else {

      // 그렇지 않다면 '위로 가기' 버튼을 숨깁니다.
      backButton.classList.remove("show");
    }
  }

  // '위로 가기' 버튼의 위치를 조정하는 함수입니다.
  function fixButtonPosition() {

    // 화면의 높이를 windowHeight 변수에 저장합니다.
    var windowHeight = window.innerHeight;

    // '위로 가기' 버튼의 높이를 buttonHeight 변수에 저장합니다.
    var buttonHeight = backButton.offsetHeight;

    // 스크롤이 페이지 하단에 가까워지면
    if (
      window.scrollY + windowHeight >
      document.body.clientHeight - buttonHeight
    ) {

      // '위로 가기' 버튼을 절대 위치로 설정하고, 하단에서 -92rem 위치에 둡니다.
      backButton.style.position = "absolute";
      backButton.style.bottom = "-92rem";
    } else {

      // 그렇지 않다면 '위로 가기' 버튼을 고정 위치로 설정하고, 하단에서 2rem 위치에 둡니다.
      backButton.style.position = "fixed";
      backButton.style.bottom = "2rem";
    }
  }

  // 초기 로딩시 '위로 가기' 버튼의 표시 여부를 결정합니다.
  toggleBackButton();

  // 초기 로딩시 '위로 가기' 버튼의 위치를 조정합니다.
  fixButtonPosition();

  // 스크롤이 발생할 때마다 '위로 가기' 버튼의 표시 여부와 위치를 조정합니다.
  window.addEventListener("scroll", function () {
    toggleBackButton();
    fixButtonPosition();
  });

  // '위로 가기' 버튼을 클릭하면 페이지 상단으로 부드럽게 이동하도록 합니다.
  backButton.addEventListener("click", function (e) {
    e.preventDefault();
    window.scrollTo({ top: 0, behavior: "smooth" });
  });
});

```
---

# 😶 프로젝트 완료 리뷰
- ### 아쉬웠던 점:
  #### 1. 자바 스크립트 문법과 함수에 서툴렀음.
  #### 2. 의사소통의 부재로 작업 진행에 있어 효율적이지 못함 이로 인해 일정이 지연됨
   
    
- ### 잘한 점:
  #### 1. loop부분을 페이지 구현 마감 거의 직전까지 해결하지 못해 어떻게 검색을 해야 하는지도 몰랐는데 구글의 힘을 빌려 구조를 다시 만들어 해결함.
  #### 2. 팀원 각자가 맡은 역할을 충실히 수행하였고, 시간적 압박과 많은 어려움이 있었지만 끊임없는 노력으로 해결함.
   
    
- ### 배운 점:
  #### 1. 반응형 웹을 만드는게 어려워보여 "잘 할 수 있을까?" 라는 의문이 들고 자신감이 없었지만 막상 만들어보니 허들이 높지 않단걸 깨닫고 자신감이 많이 오름. 
  #### 2. 자바 스크립트의 이해도를 상승시키고 전보다 더 잘 활용할 수 있게 됨.
  #### 3. 원본 페이지 코드를 보는건 컨닝이라 생각하여 전혀 안보고 해볼려 했지만 그렇게 되면 문제점이 너무 많아 원본 코드를 보는데 무작정 붙여넣기가 아니라 이해하면서 따라해보니 오히려 더 이해가 빨랐음 다른사람의 코드를 보며 참고하는것도 배우는점이 많다고 생각함.

## PPT&프로토타입
### [**🔗 PPT 바로가기**](https://drive.google.com/file/d/1sXAVAAeBlcg1zeKZ0RDTccCbTNhgJsfk/view?usp=sharing) [🔗 부산 스토리 텔링 협의회 보러가기 ](https://sslee1210.github.io/JavaScriptTeamProject/index/index.html)
