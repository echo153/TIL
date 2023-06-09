# html 기초

Visual Studio Code (vscode) 프로그램을 활용하여 html로 웹사이트 구현하기 전에 html에 대한 기본 개념을 정리해보고자 합니다. 

## html, http 개념
- HTTP(**HyperText Transfer Protocol**) : client와 server 사이의 통신 규약
- HTML(**HyperText Markup Language) :** 온라인 상의 문서(document)를 만들기 위해 데이터를 구조화 시키는 언어 (개발 언어 x, 문서화 시키는 언어 o)
    - `<tag>`를 통해 hypertext 문서를 구조화 시킴 

## WEB
- web('world wide web')을 만든 이유: 다른 사람들과 정보 교환을 위한 편리성을 위함 
    - (예전에는 프로그램이 컴퓨터에 종속되어 있었다. A 컴퓨터에서 만드는 문서들은 그 컴퓨터에서만 볼 수 있었음.)

## server-client 개념
> 클라이언트가 **버튼을** 사용해서 서버에 요청을 하면 **문서로** 응답한다.(request - respond)

![client-server](./client%20server.png)
1. 어떤 문서를 응답할지 서버에서 판별하고 그 문서를 응답함
2. 클라이언트(브라우저)가 그 문서를 받아서 예쁘게 출력 



## html tag

- `<hr>`, `<br>` → 시작과 끝이 통합되어 있는 태그 (`<br/>`도 있었는데 html 5부터 `/` 표시는 안 써도 됨)
    - `<hr>` 한 줄
    - `<br>` 줄 바꿈
- `<div>` 영역
- `<p>` paragraph
- `&lt;` <
- `&gt;` >


### 블록 요소

- 줄 바꿈
- 블록 안에 텍스트, 인라인 요소 포함 가능
- 블록 안에 블록 포함 가능 (일부 불가)
    - 태그 안에 태그 있으면 순서대로 닫아야 합니다. 
    ```
        <p>  
            <div>
            </div>
        </p>```
- 브라우저의 끝에서 끝까지 다 자기의 영역이다

### 인라인 요소

- 줄 바꿈 없음
- 인라인 안에 text, in line 태그 포함 가능
- 인라인 안에 블록 요소 포함 불가 (가능하나 지양할 것!)


### 테이블
> <table border="1"></table>
- thead, tbody, tfoot 작성 순서 상관 없음 
- `<th>` 가운데 정렬, 볼드
- `<td>` 왼쪽 정렬


## 유용한 참고 자료 
- 모르는 것 있을 때마다 보면 좋을 듯한 웹사이트들:
    - https://www.w3.org/
    - https://developer.mozilla.org/en-US/
    - https://www.w3schools.com/