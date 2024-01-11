# 🍅 팀프로젝트
## 🎯 프로젝트 목표

#### 1. 다양한 이미지를 활용하여 디자인을 구현할 수 있다.
#### 2. 팀원들 간의 활발한 소통으로 원활한 의견 교환이 이루어 질 수 있게 한다.
#### 3. 홈페이지에 필요한 기능들을 파악한 후 필요한 능력을 학습하여 개인의 능력을 증진시킨다.
#### 4. GITHUB를 통해 파일을 공유하여 GITHUB 활용 능력을 기른다.
#### 5. 정해진 시간 내에 홈페이지를 최대한 흡사하게 구현한다.
---
### ⏱ 개발 기간: 2023.10.25 ~ 2023.11.12

---

## 🛠 사용 기술 및 도구
#### **프로젝트 관리:** `Github` `Figma` `Notion` `PowerPoint`
  
#### **Tool:** `JavaScript` `vscode`

#### **사용기술:**  `Swiper` `Animation`

---
   
## 2. 팀원 및 역할 담당
#### **이성수:** (sub3) 페이지 구현, Header와 Footer 영역 구현, 전체 파일 관리, 요구분석과 구조분석 작성, PPT 제작

#### **성영은:** (sub2) 페이지 구현, GITHUB 관리, 퍼블리싱 가이드 작성, 프로젝트 보고서 작성

#### **이현범:**  (sub1) 페이지 구현, PPT 제작

#### **허수인:** (index) 페이지 구현, PPT 제작, PPT 발표

---

##📍 작업 순서
#### 1. 레퍼런스 사이트 선정
#### 2. 각 어떤 페이지 구현할지 담당 페이지 분담.
#### 3. 구현하기 전 figma로 mobile, pc버전 마크업
#### 4. 홈페이지 구현에 필요한 공용으로 들어가는 부분 asstes 폴더에 정리 (font, common … )
#### 5. 각자 맡은 페이지 구현 작업 (html → css → js 순서)
#### 6. 각자 완성된 페이지 연결작업
#### 7. 연결 후 일어나는 오류와 위치값 수정
#### 8. 작업 마무리 및 발표 준비

---
  
## 6. 퍼블리싱 가이드

### 공통사항
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
---
    
### HTML

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
 
---

### CSS

- 폰트와 아이콘 등 중복되는 소스는 assets 폴더를 이용하여 공유한다.
- 컬러는 #컬러코드와 소문자를 이용하여 작성.

```
#FF5C9B, rgb(225,92,155) ... - X
#ff5c9b - O
```

- 사이즈 값은 상황에 따라 rem, vw를 혼용하여 사용한다.
- 값이 “0”인 경우에는 단위를 생략한다.
- 선택자 작성 시 하위 선택자 작성 방식을 사용한다.
 
---

### JAVA SCRIPT

- 기본적으로 큰 따옴표(””)를 사용하고 필요 시에만 백틱(``)을 사용한다.
- const를 사용하여 모든 지역 변수를 선언. 변수를 다시 할당해야 할 경우에만 let을 사용하고 var의 사용은 지양한다.
- 선언 시 이름은 html에서 사용한 선택자 명을 바탕으로 카멜 표기법으로 작성한다.

```
const kitTitle = document.querySelector(".kit_title");
```

- 필요한 경우 코드 옆에 주석을 달아 현재 코드가 어떤 기능을 하고 있는지 설명한다.

---
   
## 5. 디렉토리 구조 분석
    
   ![앗!츄~구조분석](https://github.com/sslee1210/JavaScriptTeamProject/assets/142865231/8e132484-826c-4a1c-808d-750a6ddde20c)
   
---

## 6. 요구 분석

![앗!츄~요구분석](https://github.com/sslee1210/JavaScriptTeamProject/assets/142865231/0fdd11c2-c5c2-4d37-8d49-007efd0c3053)

---  

# 🎈 프로젝트 회고


## 문제 및 해결

### 상황 1
  - #### 문제 발생:
     데이터를 저장하거나 불러올 방법이 없어 새로고침을 누르거나 창을 나가면 저장했던 데이터가 초기화 되었습니다

      
  - #### 원인 파악:
     데이터를 저장하는 로컬 스토리지가 없었습니다

      
  - #### 문제 해결:
     로컬 스토리지를 만들고 handleId, handlePassword로 입력한 아이디와 비밀번호를 각각 ID, PW 상태에 저장, useState를 사용하여 ID와 PW를 관리했습니다



**1. 페이지가 로드될 때 로컬 스토리지에서 유저 정보를 불러옴**

```
  useEffect(() => {

   // 로컬 스토리지에서 "user" 항목의 값을 가져옴
    const savedUser = localStorage.getItem("user");
    if (savedUser) {
      navigate("/fridge");
    }
  }, [navigate]);

  // ID 입력 값이 변경될 때 호출되는 핸들러
  const handleId = (e) => {
    setId(e.target.value); // 입력 값을 ID 상태에 저장
  };

  // 비밀번호 입력 값이 변경될 때 호출되는 핸들러
  const handlePassword = (e) => {
    setPw(e.target.value); // 입력 값을 비밀번호 상태에 저장
  };
```


**1-1. 로그인 버튼을 클릭했을 때 호출되는 핸들러**
```
  const handleLogin = () => {

   // 로컬 스토리지에서 "users" 항목의 값을 가져와서 파싱
    const users = JSON.parse(localStorage.getItem("users"));
    const user = users?.find(

      // ID와 비밀번호가 모두 일치하는 유저를 찾음
      (user) => user.username === id && user.password === pw
    );

    if (user) { // 일치하는 유저가 있는 경우
      alert("로그인 성공!");

      // 로그인한 유저의 정보를 로컬 스토리지에 저장
      localStorage.setItem("user", JSON.stringify(user));
      navigate("/fridge");
    } else {
      alert("로그인 실패. 아이디 또는 비밀번호를 확인해주세요.");
    }
  };
```


### 상황 2
  - #### 문제 발생:
     캘린더를 통해 지정된 날짜에 등록한 식료품을 나타내는 기능이 구현되지 않았습니다
      
  - #### 원인 파악:
     사용 중인 캘린더 플러그인이 우리가 의도한 기능을 구현하지 못하는걸 알게 되었습니다
      
  - #### 문제 해결:
     full-calendar 라는 다른 플러그인을 사용하여 플러그인이 가지고 있는 날짜에 따른 이벤트를 띄우는 기능을 통해 원하는 기능을 구현 했습니다
    
**2. FullCalendar 라이브러리 설치**
```
npm install @fullcalendar/react @fullcalendar/daygrid
```

**2-1. FullCalendar에서 사용할 이벤트 배열 생성**
```
const eventArray = foodList.map((item) => {
   const endDay = new Date(item.expirationDate);
   const today = new Date();
   const timeDiff = endDay.getTime() - today.getTime();
   const daysDiff = Math.ceil(timeDiff / (1000 * 3600 * 24));

return {
   category: item.category,
   title: item.foodName,
   start: item.purchaseDate,
   quantity: item.quantity,
   endDay: item.expirationDate,
   dDay: daysDiff >= 0 ? `D-${daysDiff}` : `D+${Math.abs(daysDiff)}`,
     };
  }); setEvents(eventArray);
}, []);
```

**2-2. FullCalendar 컴포넌트를 사용하여 캘린더 렌더링**
```
<FullCalendar
   plugins={[dayGridPlugin, interactionPlugin]} // 사용할 플러그인 목록을 배열로 전달
   initialView="dayGridMonth" // 캘린더가 처음 로드될 때의 뷰 설정
   events={events} // 캘린더에 표시할 이벤트 정보를 배열로 전달
   headerToolbar={{ // 캘린더 상단의 툴바 레이아웃 설정
   left: "prev",
   center: "title",
   right: "next",
   }}

  dateClick={handleDayClick} // 날짜를 클릭했을 때 실행할 함수 전달
  height={400} // 캘린더의 높이 설정
/>
```


### 상황 3
  - #### 문제 발생:
     다른 팀원이 맡은 부분인 Food 페이지에서 식료품 수정을 하고 나서 새로고침을 해야 리스트가 업데이트 되는 점과 수정 시 원래의 값들이 뜨지 않는 문제점들이 생겼습니다
      
  - #### 원인 파악:
     원인 파악이 되어있지않아 직접 확인을 해봤어요 수정 컴포넌트를 모달창으로 띄우는 방식에서 데이터를 불러오는 경로가 꼬인거 같다는 생각이 들었습니다
      
  - #### 문제 해결:
   - 결국 코드를 싹 다 갈아엎고 처음부터 다시 작성했습니다
   - useEffect Hook을 사용하여 로컬 스토리지와 상태 업데이트 관리했습니다
   - 로컬 스토리지에 'foodList'라는 키로 식품 목록을 문자열 형태로 저장하고 foodList에서 주어진 food와 같은 항목을 찾아 그 인덱스를 반환하며 해결 했습니다



**3. useEffect Hook을 사용하여 로컬 스토리지와 상태 업데이트 관리**
```
  useEffect(() => {
    localStorage.setItem("foodList", JSON.stringify(foodList));
    setSortedFoodList(foodList);
  }, [foodList]);

// 식료품 수정 모달 열기 함수
  const openModal = (food, index) => {

    // 수정 중인 음식의 인덱스 및 내용 설정, 모달 열기
    const foodIndex = foodList.findIndex((f) => f === food);
    setEditingIndex(foodIndex);
    setEditingFood({ ...food });
    setIsModalOpen(true);
  };

  // 식료품 수정 모달 닫기 함수
  const closeModal = () => {
    setIsModalOpen(false);
  };

// 변경된 내용 저장 함수
const saveChanges = () => {

  // 수정된 식료품 정보로 목록 업데이트, 모달 닫기, 기존 식료품 목록을 복사하여 새로운 배열을 생성
  const newList = [...foodList];

  // 수정된 식료품을 해당 인덱스에 덮어씌움
  newList[editingIndex] = editingFood;

  // 식료품 목록을 새로운 목록으로 설정
  setFoodList(newList);

  closeModal();
};
```


**3-1. 식료품 수정 모달창**
```
      // isModalOpen이 참일 때만 모달을 표시
      {isModalOpen && (
        <div className={styles.modal}>
          <div className={styles.modalBox}>
            <img
              src={path + "/images/food_back_blue.svg"}
              alt="뒤로가기"
              className={styles.back}
              onClick={closeModal}/>
            <h2>싱싱고 수정하기</h2>

        // setEditingFood 함수를 호출하여 editingFood 상태의 category 값을 업데이트
            <label>
              <select
                value={editingFood.category}
                onChange={(e) =>
                  setEditingFood({ ...editingFood, category: e.target.value })}>
                {categoryOptions.map(
                  (category, index) =>
                    category !== "전체" && (
                      <option key={index} value={category}>
                        {category}
                      </option>
                    ))}
              </select>
            </label>

        // 입력된 값이 변경되면 setEditingFood 함수를 호출하여 수정된 식료품 값으로 업데이트
            <label className={styles.editName}>
              <span>식재료명</span>
              <input
                type="text"
                value={editingFood.foodName}
                onChange={(e) =>
                  setEditingFood({ ...editingFood, foodName: e.target.value })
                }/>
            </label>

        // 입력된 값이 변경되면 setEditingFood 함수를 호출하여 수정된 수량 값으로 업데이트
            <label className={styles.editNum}>
              <span>수량</span>
              <input
                type="number"
                value={editingFood.quantity}
                onChange={(e) =>
                  setEditingFood({ ...editingFood, quantity: e.target.value })
                }
                required/>
            </label>

        // 입력된 값이 변경되면 setEditingFood 함수를 호출하여 수정된 구매일과 소비기간 값으로 업데이트
            <div className={styles.dateBox}>
              <label>
                <span>구매일</span>
                <input
                  type="date"
                  value={editingFood.purchaseDate}
                  onChange={(e) =>
                    setEditingFood({
                      ...editingFood,
                      purchaseDate: e.target.value,
                    })}required/>
              </label>

              <label>
                <span>소비기간</span>
                <input
                  type="date"
                  value={editingFood.expirationDate}
                  onChange={(e) =>
                    setEditingFood({
                      ...editingFood,
                      expirationDate: e.target.value,
                    })}required/>
              </label>

        // 입력된 값이 변경되면 setEditingFood 함수를 호출하여 수정된 메모 값을 업데이트
            </div>
            <label className={styles.editMemo}>
              <span>메모</span>
              <textarea
                value={editingFood.note}
                onChange={(e) =>
                  setEditingFood({ ...editingFood, note: e.target.value })
                }/>
            </label>
```



### 상황 4
  - #### 문제 발생:
     로컬 스토리지로는 각 사용자마다 다른 식료품 목록을 보여주는 구현이 어려웠습니다 ( 저장된 데이터에 다른 데이터를 연결하는 부분이 잘 되지 않았습니다)
    
  - #### 원인 파악:
     데이터베이스(ex.몽고DB)를 이용하여 서버 연결을 통해 회원정보와 데이터 정보를 연결해야 했습니다
      
  - #### 문제 해결:
     프로젝트가 끝난 후 혼자 독학하며 연결하기로 했습니다



### 상황 5
  - #### 문제 발생:
     어색한 분위기에 서로 소통도 잘 안되어 역할을 분담하거나 개개인의 작업 진행 상황을 판단하지 못하였습니다
      
  - #### 원인 파악:
     처음 본 사람들끼리 이루어진 팀이라 서로 낯가림이 심했습니다
      
  - #### 문제 해결:
     용기를 내 팀원들에게 먼저 다가가 단톡방을 만들고 대화를 주도하여 친밀감을 형성시키고 밝은 분위기로 회의를 이끌어 좋은 분위기에서 프로젝트를 마칠 수 있었습니다


# 프로젝트 완료 리뷰
- ### 아쉬웠던 점:
  #### 1. 리액트를 활용함에 어렵고 서툴렀던 탓에 프로젝트 진행 속도가 늦어졌습니다
  #### 2. 낯을 많이 가리는 성격이라 팀원들과 좋은 팀워크를 이루지 못할 거라 생각했습니다
   
    
- ### 잘한 점:
  #### 1. 잠을 줄이고 공부 시간을 더 늘려 코딩 능력을 더 향상시키고 리액트를 활용함에 보다 더 능숙해 졌습니다
  #### 2. 처음엔 낯을 좀 가렸지만 용기를 내 팀원들에게 먼저 다가가 결국 팀원들과의 원활한 커뮤니케이션 및 협력을 통해 프로젝트를 성공적으로 완성 시킬 수 있었습니다
   
    
- ### 배운 점:
  #### 1. 리액트와 관련한 기술적 이해도를 상승시키고 기간 내에 프로젝트를 마무리 지을 수 있었습니다
  #### 2. 처음 만난 사람과의 친밀감을 형성하는 법을 알게 되어 팀원들과의 원활한 커뮤니케이션으로 협업 능력을 향상시켰고 밝은 팀 분위기를 유지하였으며, 팀원들을 이끌 수 있는 리더십 능력을 키울 수 있었습니다

# 프로젝트 바로가기
## [🔗 부산 스토리 텔링 협의회 ](https://sslee1210.github.io/JavaScriptTeamProject/index/index.html)
