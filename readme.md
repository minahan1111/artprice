# Topic : '미술품이 갖는 특징과 경제적 지표를 고려한 국내 작가들의 미술품 경매 가격 예측'



## Researcher : 김종백, 한민아



## Data

1. Feature
    1. 미술품의 특징
        1. 작가, 재질, 제작연도, 규격, 장르, 기법, 거래일…
        2. K-artprice 사이트에서 크롤링 가능(로그인 필요)
        3. ![image-20211113160048685](readme.assets/image-20211113160048685.png)
    2. 경제적 지표
        1. KOSPI, Bitcoin Price, 서울지역 부동산 매매 평균가격, 원달러 환율, 유가
            1. KOSPI : KRX 데이터센터에서 확보
            2. BTC Price
                1. 2017-09 ~ 2021-11-12까지의 Upbit BTC/KRW 가격
                2. 2016-01 ~ 2021-11-12까지의 Coinbase BTC/USD 가격
            3. 부동산 매매 지표 : KB 월간주택가격동향 데이터 참조
            4. 원달러 환율 : investing.kr 에서 확보
            5. 유가 : 서부텍사스산중질유(WTI) 선물 가격 확보
        2. 일별 데이터는 investing.kr 등에서 확보 가능
    
2. Label
    1. 낙찰 가격
    2. K-artprice에서 확인 가능



## Target Artist

분석 작가명(K-artprice사이트 작가별 낙찰총액 순위 중 국내 작가들 상위 30명) : 

김환기, 이우환, 박서보, 정상화, 김창열, 박수근, 천경자, 이중섭, 윤형근, 이대원, 

유영국, 장욱진, 김종학, 백남준, 오치균, 하종현, 도상봉, 이강소, 이왈종, 정선, 

김홍도, 김태호, 이상범, 남관, 이응노, 전광영, 김정희, 서세옥, 이성자, 김기창(총 30명)

 

# Preprocessing

## 데이터 결합

- 시계열 데이터와 경매 낙찰 가격에 대한 데이터 결합 필요

## 데이터 결측치 제거

## 데이터 범주 기준 정의

