# 2019.01.01 (Lpoint 공모전)



## 1. 데이터셋 구성 방법

1. 날짜 기반 데이터셋

   1. 주어진 기간의 데이터들로 구성 후 이를 train/test set으로 구분
   2. 주어진 기간 이상의 데이터로 구성 후 4~9월은 train, 그 이상은 test로 구분 

2. 상품 기반 데이터 셋

   1. 타겟 상품들을 위주로 해당 상품과 관련된 데이터들로 데이터셋 구성

3. 고객정보 기반 데이터 셋

   1. 고객 집단과 관련된 데이터들로 데이터셋 구성

4. 위의 3가지 방법들의 조합

   1. 날짜 + 상품
   2. 날짜 + 고객정보
   3. 상품 + 고객정보
   4. 날짜 + 상품 + 고객정보


## 2. 데이터셋에 들어갈 정보들

1. 브랜드 + 소분류
2. 날짜
3. 고객정보
4. ~~날씨(외부데이터)~~
5. sns 데이터
6. 검색 데이터



## 3. 데이터에서 활용 가능한 정보

- 브랜드 + 소분류
- 날짜
- 고객정보(custom 데이터)
  1. 성별
  2. 연령대
  3. 가입여부
  4. 사용 기기(데스크탑/모바일/태블릿)
  5. 접속 지역
- 고객정보 (소비 패턴)
  1. 세션시간
  2. 페이지 뷰 수
  3. 히트 수
  4. 검색어 수 
  5. 검색량



## 4. 활용할 외부 데이터

- ~~날씨~~

> ~~kweather([링크](http://www.kweather.co.kr/kma/kma_past.html?))를 이용해 수집 가능(월별, 지역별)~~

- 트렌드
  1. 각 상품의 검색 트렌드
  2. 각 상품의 쇼핑 트렌드
  3. 관련 유튜브 영상 데이터 

> 네이버 데이터랩(통합검색어 트렌드) API([링크](https://developers.naver.com/docs/datalab/search/))활용
>
> 네이버 데이터랩(쇼핑인사이트) API([링크](https://developers.naver.com/docs/datalab/shopping/))활용
>
> Youtube data API([링크](https://developers.google.com/youtube/v3/getting-started?hl=ko#resources))활용

- 일간 이벤트 데이터
  1. ~~인스타그램 태그를 통해 이벤트 날짜 추정~~

> ~~instagram API([링크](https://github.com/facebookarchive/python-instagram))~~  (인스타/ 페이스북은 포기해야 할 듯... api 인증이 안됨..)
>
> 인스타 / 페이스북 대체 페이지([링크](https://pikdo.net/u/styleandstar/2064045967))

- 이벤트 정보
  1. 이벤트(만우절, 불꽃축제, 휴가시즌 등...)