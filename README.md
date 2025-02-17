# 유투브 9din Vue3 무료 강의
[9Din 유투브 강의 재생목록 링크](https://www.youtube.com/watch?v=wCyF_bU9X0I&list=PL-cIzvS-5d-1httQSLn0rd3FIlwf-uMYF&index=2)  
Vue2 기반 OptionsAPI 기본문법 적용 후 CompsotionAPI 문법을 간단하게 적용해본다.

# Vue.js란?
<details>
<summary>펼치기/접기</summary>
<br>

웹 사용자 인터페이스를 만들기 위한 쉽고 강력하며 다재다능한 프레임워크이다.  
웹 프론트엔드 시장에서 가장 많이 사용되는 스택은 React 이고, 그 다음으로 Vue.js이다.  
후발주자로 Svelte가 빠르게 치고 올라고오 있으나, 아직 React와 Vue.js를 대체할 수준까진 아니다.
Vue.js를 선택하는 이유는 접근성과 낮은 러닝커브이다.  
웹 개발을 처음 시작한 사람들, 초보자들에게 Vue.js라는 선택지는 쉽게 접근할 수 있고 쉽게 입문할 수 있다는 가장 큰 장점이 있다.  
그러나 쉽다고 퍼포먼스가 전혀 낮은것은 아니다.  
다른 프론트엔드 툴과 견주어도 절대 뒤쳐지지 않는 성능을 낼 수 있다.  
그렇기에 메인 툴로 선정하여도 훌륭한 선택지가 될 수 있다.  

Vue.js는 프레임워크이다.  
리액트는 사용자 인터페이스를 만들기 위한 자바스크립트 라이브러리라고 표현하고 있다.  
라이브러리는 개발자들이 개발을 최소한으로 편리하게 하기 위해 만든 모듈이다.  
가구에 빗대어 표현해보자면, 라이브러리는 어떤 책상을 만드는데 필요한 재료들이라고 생각하면 된다.  
반면 프레임워크는 이러한 가구들이 미리 조립되어있는 상태를 말하며 가구들을 활용하여 리모델링을 이룬다.  
이처럼 프레임워크는 라이브러리의 집합체 더 큰 개념이라고 이해하면 된다.  
따라서 라이브러리같은 경우에는 기능상의 통제권이 개발자, 즉 사용자에게 있는 반면 프레임워크는 통제권이 프레임워크에 있다.  
따라서 프레임워크는 큼직한 기능들이 미리 세팅되어 있는 완성형 도구라고 생각하면 된다.  
그러므로 Vue.js는 타 개발도구들 보다 자유도는 비교적 낮을 수 있지만 협업에 있어 약속된 기능들을 사용하기 때문에 코드가 명시적이라는 장점이 있다.  

다음으로 Vue.js의 구조를 알아보자.  
Vue.js의 구조는 딱 2가지만 알고있으면 된다.  
첫번째로는 `SPA` 구조라는것 두번째로는 `SFC` 구조라는것

먼저 `SPA` 구조는 `Single Page Application`의 약자로 말 그대로 하나의 페이지에서 유저가 원하는 정보만 보여주는 방식이다.  
페이지를 구성하는 HTML파일이 하나만 있다는것을 의미한다.  
HTML파일 안에서 사용자가 요청하는 페이지의 정보만 불러오는 구조라고 이해하면 된다.  
즉, 하나의 HTML파일의 body태그 안에서 보여지는 것들이 유저의 요청에 의해서 바꿔치기 되는 형식이다.  

다음으로는 `SFC` 구조이다.  
Vue.js 확장명은 .vue이다.  
해당 파일 안에서 HTML, CSS, JS가 관리된다.  
하나의 컴포넌트 안에서 이 모든게 관리가 된다고 하여 `Single File Component`라고 부른다.  

- 경로/컴포넌트명.vue
  ```vue
  ```

</details>
<br>

# Vite기반 Vue3 프로젝트 세팅
<details>
<summary>펼치기/접기</summary>
<br>

1. 설치 명령 입력
  ```
  PS C:\프로젝트설치 상위경로> npm create vite@latest
  ```

2. 프로젝트명 입력
  ```
  PS C:\Programming\workspace_vs> npm create vite@latest
  ? Project name: » {프로젝트명}
  ```

3. 프레임워크 Vue 선택
  ```
  PS C:\Programming\workspace_vs> npm create vite@latest
  √ Project name: ... vue3-vite-9din-basic
  ? Select a framework: » - Use arrow-keys. Return to submit.
      Vanilla
  >   Vue
      React
      Preact
      Lit
      Svelte
      Solid
      Qwik
      Angular
      Others
  ```

4. 사용 언어 Javascript 선택
  ```
  PS C:\Programming\workspace_vs> npm create vite@latest
  √ Project name: ... vue3-vite-9din-basic
  √ Select a framework: » Vue
  ? Select a variant: » - Use arrow-keys. Return to submit.
      TypeScript
  >   JavaScript
      Official Vue Starter ↗
      Nuxt ↗
  ```

5. 설치 완료 후 출력문
  ```
  Scaffolding project in C:\Programming\workspace_vs\vue3-vite-9din-basic...

  Done. Now run:

    cd vue3-vite-9din-basic
    npm install
    npm run dev
  ```
  
6. Node.js 의존성 라이브러리 설치
  ```
  npm install
  ```
  
7. 서버 기동
  ```
  npm run dev
  ```
</details>
<br>

# 템플릿1
<details>
<summary>펼치기/접기</summary>
<br>

- 경로/컴포넌트명.vue
  ```vue
  ```

</details>
<br>

# 템플릿2
<details>
<summary>펼치기/접기</summary>
<br>

  ## 세부
  <details>
  <summary>펼치기/접기</summary>
  <br>

  - 경로/컴포넌트명.vue
    ```vue
    ```
  </details>

  ## 세부
  <details>
  <summary>펼치기/접기</summary>
  <br>

  - 경로/컴포넌트명.vue
    ```vue
    ```
  </details>

</details>


