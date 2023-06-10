# form

## 하이퍼링크 기초 

`http://127.0.0.1:5500/web01-html/html10-form-res.html?id=%E3%84%B4%E3%85%87%E3%84%B9&pw=%E3%85%87%E3%84%B9sdf&rdo=n&web=web&etc=%E3%85%81%E3%84%B4%E3%84%B9%E3%84%B4%E3%85%87` 

- 클라이언트 서버 request 하는 것을 복귀해봅시다. 하이퍼링크를 보면 '?' 뒤에 있는 것을 query string 이라고 하고, '=' 표시로 입력된 내용이 뜹니다
- header : 우리가 링크에서 볼 수 있는 내용
- body : 안 보이는 내용 


## form 태그와 속성

`<form action="html10-form-res.html" method="get">`

- form 태그 : 데이터를 많이 전달할 때 사용 (form tag 안에 있는 것들이 전달됨)

- 속성:

    - `action=""` : 어디로 전달할 것인지 url 표시 

    - `method` : 입력한 데이터의 전송 방식 (get/post) 설정 
        - get : 원래는 데이터 요청할 때 사용되었지만, 지금은 데이터가 링크에 보여도 상관 없을 때에 사용됨!
            - 링크의 header 부분에 어떤 데이터가 전송되는지 표현되기 때문에 보안에 취약함 
        - post : 원래는 데이터 저장시키고 싶을 때 사용되었지만, 이제는 데이터 전송할 때 링크에 보이면 안 될 때 사용! (숨김 처리 하고 싶을 때)
            - 링크의 body 부분에 저장되어서 전송 되니 표면상에 보이지 않음 
            - 글자 수 제한 없음
        - rest / restful (자주 안 씀)
            - put 
            - delete
    - `type` : 입력 양식 모양 


### 웹페이지의 개발자 메뉴에서 확인하는 방법
1. 개발자 메뉴 > Network > 전송 버튼 누르면 왼쪽에 Name 뜸
2. Headers, Payload etc 확인 가능
    - payload 에 전달 내용 볼 수 있음 


## input 태그

- input의 `name` 속성이 붙어 있는 애들의 value 값이 전달된다.
    - input 박스 안에 작성한 내용이 value로 전달됨 

- input 외에도 태그가 많음

### input type:

- radio : n개 중 하나만 선택 가능

- checkbox : 체크한 name의 value 전달

- submit : 'submit 이벤트'가 발생해서 form 태그에서 지정했던 action 링크로 정보를 전송함
    
- select : 선택 가능한 항목 
    
    ![select](/TIL-html/images/select.png)

    ```html
    <!-- select 코드: -->
    <select name="lunch">
            <option value="kimbab">김밥</option>
    ```

- optgroup : 선택할 수 없지만 표시됨 

    ![optgroup](/TIL-html/images/optgroup.png)
    
    ```html
    <!-- optgroup 코드: -->
    <select name="dinner">
            <optgroup label="한식">
                <option value="dakbokkeumtang">닭볶음탕</option>
    ```

- get 양식 제출 후 url 링크를 확인해보면 선택한 value가 전달됨 
    
    `http://127.0.0.1:5500/web01-html/html10-form-res.html?lunch=kimbab&dinner=dakbokkeumtang`


