# HTML과 CSS 기초
## HTML

1. 기본구조
```html
<!DOCTYPE html>
<html lang="ko-KR">
  <head>
    <meta charset="UTF-8">
    <title>문서제목</title>
  </head>
  <body>
    html의 기본 구조 관련 명령어에 대해 학습했습니다.
  </body>
</html>
```
---
2. 제목관련 요소

```html
<h1>대제목</h1>
<h2>중제목</h2>
<h3>소제목</h3>
```

>h1 요소부터 h6 요소까지 총 6단계를 사용할 수 있으며 중간에 단계를 건너뛰어서 제공하여서는 안된다.

3. 텍스트 관련 요소

* 굵게 기울임꼴 (b, i)
* 강한강조와 강조 (strong, em)
* 줄바꿈 및 수평선 (br, hr)
* 인용 (blockquote, q)
* 약어와 머릿글자 (abbr)
* 주소정보 (address)
* 특수문자 (예 - 공백문자)

4. 목록 관련 요소

* 비순서형 목록 (ul, li)
* 순서형 목록 (ol, li)
* 정의형 목록 (dl. dt, dd) - 백과 사전

5. 하이퍼링크와 이미지
```html
<ul>
    <li><a href="https://www.multicampus.com/main">멀티캠퍼스</a></li>
    <li><a href="https://www.facebook.com/multicampusHRD/" title="멀티캠퍼스" target="_blank">페이스북</a></li>
    <li><a href="./04_list.html">목록 요소</a></li>
    <li><a href="#heading2">이미지로 제목으로 이동</a></li>
  </ul>

  <p>
  <img src="./assets/logo.gif" alt="From A To Zucchini" width="458" height="75">
  </p>
```

* 멀티캠퍼스(https://www.multicampus.com/main)
* [멀티캠퍼스](https://www.multicampus.com/main)
* ![From A to Zucchini](./html/assests/../assets/logo.gif)

6. 테이블

* 테이블 영역 (table)
* 테이블 행 (tr)
* 제목 셀 (th)
  + scope="col" (열 제목)
  + scope="row" (행 제목)
* 내용 셀 (td)
  + 행 병합 (rowspan)
  + 열 병합 (colspan)

```html
<table border="1">
    <tr>
      <th scope="col">구분</th>
      <th scope="col">토요일</th>
      <th scope="col">일요일</th>
    </tr>
    <tr>
      <th scope="row">티켓판매</th>
      <td>120</td>
      <td>135</td>
    </tr>
      <th scope="row">매출</th>
      <td>$600</td>
      <td>$675</td>
  </table>
```

7. 폼 관련 요소

* 폼 그룹 (form)
    + action (서버 URL)
    + method (GET 또는 POST)
* 연관성 있는 서식의 묶음 (fieldset)
* 서식의 묶음의 성격을 명시 (legend)
* 폼 서식 (input, select, texarea)
* 전송 버튼 (button)

## CSS
### CSS 규칙(rule set)
```css
selector {
  property : value;
}
```
### CSS 적용하는 방법
* Exteral Style Sheet(외부 스타일 시트)
* Embedded Style Sheet(내부 스타일 시트)
* Inline Style Sheet(인라인 스타일 시트)

### CSS의 3가지 개념
* 상속(Inheritance)
* 겹침(Cascade)
* 구체성(Specificity)

### CSS 다양한 선택자
* 요소 선택자 (h1, p, div ....)
* 클래스 선택자 (.class명)
* 아이디 선택자 (#id)
* 그 외 다양한 선택자가 있음.

### CSS의 다양한 속성
* 색상
  + color(글자색)
  + background(배경색)
* 텍스트
  + 글꼴(font-family)
  + 글자크기(font-size)
  + 기울임꼴 여부(font-style)
  + 글꼴 굵기 설정(font-weight)
  + 줄 간격 (line-height)
  + 대소문자 변환 (text-transform)
  + 텍스트 장식 여부 (text-decoration)
  + 글자 그림자 (text-shadow)
* 박스 (display, box-sizing)
  + 가로 크기(weith)
  + 세로 크기 (height)
  + 안쪽 여백 (padding)
  + 테두리 (border)
  + 바깥쪽 여백 (margin)
* 레이아웃
  + position : static
  + position : relative
  + position : absolute
  + position : fixed
  + float : left
  + float :right