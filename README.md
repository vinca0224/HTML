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