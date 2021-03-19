# 0319
## DB에서 특정 날짜 출력하기
```sql
select sum(dntprice) from donation where TO_CHAR(dntdate,'yyyy-mm-dd') > '2021-03-16' order by dnt_paynum asc;
```
- **sysdate로 데이터를 입력했을 때 DATE자료형은 시분초 까지 있기 때문에** '2018/12/03 17:29:59' 이런식으로 데이터 삽입이 됨 
<br> 그래서 형식까지 변경해주기 위해 'YYYYMMDD'를 붙여주는 것! → 이렇게 바꿔줬을 때 원하는 날짜를 검색할 수 있다
