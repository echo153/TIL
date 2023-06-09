# html 문서 기본 구조

## 기본 태그 설명 
- `<!DOCTYPE html>` : 현재 문서의 html 타입을 html5로 명시
- `<html>` : html 문서의 시작과 끝을 표시 
- `<head>` : 웹 페이지 문서에 대한 정보로, 메타데이터를 정의 
    - `<title>` 문서 자체에 표시는 안 되어 있고, 브라우저 탭에 보이는 제목
- `<body>` : 웹 페이지의 실제적인 내용 (content)를 작성 
- `<br>` : 줄 나누기 / 줄 바꾸기 
- `<address>` : 주소 태그


## body 태그와 속성 
- 태그 : `<a href='링크주소'>링크</a>`
    - 태그 이름 : `<a>`
    - 속성명 : href
    - 속성값 : 링크주소
    - 내용 : 링크 

## html 주석 
> <!-- 주석, comment -->

- 맥북 바로가기 shortcut: `cmd + /` 

## 앵커 태그
- `<a>` : 다른 사이트나 같은 페이지의 다른 위치로 이동하는 하이퍼링크
    - `<a href="#content1">Content 1</a>` 처럼 #을 붙여 주면 같은 페이지의 지정된 위치로 이동할 수 있습니다. 

## 리스트 태그 
- ul : unordered list
    > <ul style='list-style-type: circle'>
    이렇게 bullet point 자체의 스타일도 지정할 수 있습니다. 

- ol : ordered list
    ```
    <ol>
        <li>항목 1</li>
        <li>항목 2</li>
    </ol>

    <ol type="I">
        <li>항목 1</li>
        <li>항목 2</li>
    </ol>
    ```
    - type 속성을 바꿔서 roman numeral, ABC 등으로 바꿀 수도 있습니다. 

- dl : definition list 
    - dt : definition title
    - dd : definition description
    ```
    <d1>
        <dt>HTML</dt>
        <dd>웹 페이지를 위한 마크업 언어</dd>
    </d1>
    ```

## 테이블 태그 

    <table>
        <tr>