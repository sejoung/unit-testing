# 단위 테스트(생산성과 품질을 위한 단위 테스트 원칙과 패턴)

Rider에 mono를 설치해야 한다.

To run integration tests:

1. Use the script in DatabaseGenerationScript.sql to create the database.
2. Configure the tests to execute sequentially, not in parallel.


## 9 장 테스트를 위해 로컬에 mssql 서버 기동하기

```
docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=eksdnlxptmxm1@" \
   -p 1433:1433 --name mssql --hostname mssql \
   -d \
   mcr.microsoft.com/mssql/server:2022-latest
````

sa/eksdnlxptmxm1@ 로 접속한다.

DatabaseGenerationScript.sql 파일을 실행해서 테스트용 테이블 및 데이터 베이스를 만든다

* [단위 테스트(생산성과 품질을 위한 단위 테스트 원칙과 패턴)](http://www.acornpub.co.kr/book/unit-testing)
