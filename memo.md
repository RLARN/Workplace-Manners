# 수업 매모장.
3학년2학기 성용우 교수님 수업

* ```box-sizing: border-box;``` 보더를 안쪽으로  

* 사이즈가 600보다 작으면 flex 정렬을 colum으로 해라
    ```css
    @media all and (max-width: 600px) {
        .flex-container{flex-direction: column;}
    }
    ```

* 중간고사는 2주 연기! >> 11월 4일
* cursor : pointer; 호버시 손꾸락
* margin: auto 정가운데로 정렬  
* flex 안내 사이트  
https://d2.naver.com/helloworld/8540176


* 말줄임표 공식 (아래 3개 코드 다 작성)
    ```css
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
    ```
    
* 10월 마지막주 수행평가  
* 아이콘 복붙 사이트  
https://copychar.cc

*   사이즈 보존 (Flex 에서 모양 안찌그러지게)
    ```css
    flex-shrink:0;
    ``` 
    
*   돌려버리기
    ```css
    transform: rotate(45deg);
    ```

* 이미지넣기
    ```css
    figure
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    ```
* 한줄 줄이기
    ```css
    overflow: hidden; text-overflow: ellipsis; white-space: nowrap; flex-grow: 1;
    ```

* 여러 줄 말줄임 속성 값 (2줄)
    ```css
    {display:-webkit-box;
    overflow:hidden;
    height:50px;
    -webkit-line-clamp:2;
    -webkit-box-orient:vertical}
    ```

* rem :16px
* em : 상대값
* 수직정렬
    ```
    flex-direction: column;
    ```
* 화면크기에따른 변화 주기
    ```css
        @media all and (min-width:600px){
        .card-list-wrap{overflow-x: hidden;}
        .card-list{display: flex;flex-wrap: wrap; margin: 0 -1vw;}
        .card-item{width: 50%;padding: 0 1vw;}
        .card-btm{flex:auto}
    }

    @media all and (min-width:1200px){
        .card-item{width: 33%; flex: auto}
        .card-list{}
    }
    ```
    