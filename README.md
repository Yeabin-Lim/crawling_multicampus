# multicampus_crawling

## Project 개요
- 다양한 사이트에 있는 정보를 수집하여 크롤러를 구현하고 이를 MariaDB에 데이터를 저장 & 원하는 데이터를 추출하여 이메일로 보내는 프로젝트이다.

## Crawling web site & detail
- 네이버 랭킹 뉴스 <https://news.naver.com/main/ranking/popularDay.nhn>
  * 정치, 경제, 사회 TOP5 뉴스
  * 날짜, 기사 제목, 카테고리, 기사 내용 요약본
  
- 네이버 환율 정보 <https://finance.naver.com/marketindex/exchangeDetail.nhn>
  * 미국 USD, 유럽연합 EUR, 일본 JPY, 중국 CNY 
  
- 취업 정보(JobKorea) <http://www.jobkorea.co.kr/starter/calendar/202005>
  * 월별 채용 공고 시작일, 채용 회사
  
- 네이버 영화 정보 <https://movie.naver.com/movie/sdb/rank/rmovie.nhn>
  * 영화 제목, 날짜, 장르, 국가, 상영시간, 개봉일, 줄거리
  
- 날씨 정보 <https://www.data.go.kr/> + <https://www.weatheri.co.kr/forecast/forecast01.php>
  * 날짜, 최저기온, 최고기온, 비, 강수량, 옷차림, 날씨

- 음악 정보(Melon) <https://www.melon.com/dj/djfinder/djfinder_inform.htm>
  * 날짜, 노래, 가수, 좋아요 수

## 사용법
1. 날씨 사이트에서 API key를 얻는다.
2. google email에서 비밀번호 얻고 이메일을 보내고 받기 위한 설정을 한다. 
3. MariaDB를 설치하고 DB를 생성한다.
4. weather_crawling.ipynb에서 API key를 입력한다.
5. main.ipynb 4번째 셀에서 DB의 이름과 password를 입력하고, 11번째 셀에서 email과 password를 입력한다.
6. main.ipynb의 모든 셀을 실행시키면 된다.
7. 필요에 따라 각 * _crawling.ipynb 에서 날짜의 범위를 수정해 사용하면 된다. 
