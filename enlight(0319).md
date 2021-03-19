# 0319
## DB에서 특정 날짜 출력하기
```sql
select sum(dntprice) from donation where TO_CHAR(dntdate,'yyyy-mm-dd') > '2021-03-16' order by dnt_paynum asc;
```
- **sysdate로 데이터를 입력했을 때 DATE자료형은 시분초 까지 있기 때문에** '2018/12/03 17:29:59' 이런식으로 데이터 삽입이 됨 
<br> 그래서 형식까지 변경해주기 위해 'YYYYMMDD'를 붙여주는 것! → 이렇게 바꿔줬을 때 원하는 날짜를 검색할 수 있다

## 수정 사항
- chatiry - css - script - progressbar.js 에서 출력하지 않으려고 
**지정되어있는 값 progress + % 삭제**

```java
script -> progressbar.js

// Render the progress bar
if ( settings.animation ) {
	overlay += '<span class="bar" style="background-color:' + settings.barColor + ';"><span class="progress-percent" style="line-height:' + settings.height + 'px;">' + progress + '%</span></span>';
		}

// Render the progress bar
// 메인에서 수치  progress + % 빼고 사용
if ( settings.animation ) {
	overlay += '<span class="bar" style="background-color:' + settings.barColor + ';"><span class="progress-percent" style="line-height:' + settings.height + 'px;">' +  '</span></span>';
}
```


### 0319 느낀 점
진짜 될까..이틀째 부트스트랩 메인 적용하는데 허접한 것 같다 ㅠㅠ (템플릿이 있는데 효과를 내지 못하는 것 같음)
- 메인한다고 괜히 나댔다 헝 ㅠㅠㅠ 이렇게 할 게 많을지 몰랐고여.. 만들어놓은 템플릿 건드리는게 더 힘든 것 같음
- (임플란트해서 아프니까 더 하기싫고 더 심란...못하면 어떡하지..)

