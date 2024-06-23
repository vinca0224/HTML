# HTML

## 1일차
- 텍스트 관련 태그
    - p: 문단 만들기
    - br: 개행

- 스타일 태그
    - <style> 태그안에 디자인요소 작성
    - css 파일에 스타일을 정의하고 css 파일을 불러와 스타일을 꾸밀 수도 있다
    ```html
    <link rel="stylesheet" href="style.css"/>
    <!--rel: 속성, stylesheet: 값
            href: 속성, 위치경로-->
    ```

- a 태그
    - anchor 태그는 다른 웹페이지난 웹페이지 내부의 특정한 위치로 이동
    href 속성을 사용한다(이동할 위치)
    target 속성을 사용하면 새로운 창이 열리면서 이동된다
    - a 태그는 웹페이지로 이동하거나 웹페이지내부로도 이동이 가능하다
    - '#' : 웹표준에 따른 빈 링크를 나타낸다

## 2일차
- img, audio, video 태그

- li, ul 관련 태그

- 테이블 태그
    - table 태그로 테이블을 만든다
    tr 태그로 한 행을 구성하고 th 태그로 제목, td 태그로 셀을 작성한다
    border 속성을 사용하여 테두리를 만든다
    ```html
    <table border="1">
            <tr>
                <th colspan="2">지역별 홍차</th>
            </tr>
            <tr>
                <th rowspan="3">중국</th>
                <td>정산소총</td>
            </tr>
            <tr><td>기문</td></tr>
            <tr><td>운남</td></tr>
            <tr>
                <th rowspan="4">인도 및 스리랑카</th>
                <td>아삼</td>
            </tr>
            <tr><td>실론</td></tr>
            <tr><td>다질링</td></tr>
            <tr><td>닐기리</td></tr>
        </table>
    ```

## 3일차
- Fom 태그
    - method
        - get: 주소 url의 끝에 폼데이터를 실어 보낸다(간단하지만 보안에 취약)
        - post: 몸체에 폼데이터를 실어보낸다(어렵지만 보안에 좋다)
    - input
    - label
    - select
    ```html
        <form>
        <label for="name">user</label>
        <input type="text" id="name">
        <label for="tel">tel</label>
        <input type="tel" id="tel" placeholder="전화번호를 입력하세요">
        <hr>
        <input type="email"><br>
        <input type="color"><br>
        <input type="date"><br>
        <input type="search">
    </form>
    ```

## 4일차
- css 기초
    - css 적용 우선순위
        1. 속성값 뒤에 !important
        2. style을 직접 지정한 속성(인라인 속성)
        3. #id로 지정한 속성
        4. 태그로 지정한 속성
        5. 상위 객체에 의해 상속된 속성

- 태그 선택자
    - *(전체 선택자)
    - #(id): 중복 불가
    - .(class): 중복 가능

- 시멘틱 태그

- 블록요소, 인라인 요소
    1. 블록요소 태그 
        - html, body, div, p, ul, ol, li, dl, dt, dd ...
        - 기본 가로 공간의 크기가 부모태그와 동일하게 인식
        - 연속해서 작성하면 세로 배열
        - 공간값이 적용됨(w,h)
    2. 인라인 요소 태그
        - a, span, strong, i, em ...
        - 기본 가로 공간의 크기가 안쪽에 포함된 내용만큼만 인식(컨텐츠)
        - 연속해서 작성하면 가로 배열
    3. 인라인 블록 요소 태그
        - img, input, button ...
        - 기본 가로 공간의 크기가 안쪽에 포함된 내용만큼만 인식
        - 연속해서 작성하면 가로 배열
        - 공간값이 적용됨

## 5일차
- 반응 선택자
    - 사용자의 반응으로 hover와 active 상태가 만들어 진다.
    마우스 커서 올리기 - hover, 클릭 - active 적용

- 속성 선택자 : 선택자[속성=값]

- 상태 선택자 : 입력양식의 상태를 선택
    - :checked - 체크상태의  input 태그 선택
    :focus - 포커스를 맞춘 input
    :enabled - 사용가능한 input
    :disabled - 사용 불가능한 input

- 구조 선택자 : 특정 위치에 있는 태그를 선택할 때 사용

## 6일차
- flex
    - vh : view height : 화면에 보이는 공간을 기준 */
    - flex-direction : 기준축을 정의
    - row, row-reverse, column, column-reverse 
    - justify-content : 중심축에서 아이템의 배치를 담당
    - flex-start, flex-end, center, space-around
    - align-items : 반대축에서 아이템을 배치하는 속성

- grid
    -  display : grid를 사용하면 그리드 박스를 사용하는데,
    부모컨테이너를 grid 지정하면 자식은 grid cell이 된다
    - grid 속성 : grid-template-columns, grid-template-row, grid-template-areas
    - grid-template-columns : 100px 100px 100px -> 100px 3개 만듬
    - grid cell 속성 : grid-column-start, grid-column-end, grid-row-start, grid-row-end, 
    - repeat 키워드로 반복횟수를 설정
    - grid-template-columns:repeat(5, 20%)
    - grid-template-columns:repeat(5, 1fr)
    - grid-template-columns:repeat(5, 100px)
    - grid-auto-rows:minmax(150px, autp) -> 각 컬럼의 아이템의 크기가 다른 경우 최소높이는 150px, 너비 자동으로 늘림

## 자습 예제

[슬라이드 바]<img src="https://github.com/vinca0224/HTML/blob/main/output/gif01.gif" width="730">