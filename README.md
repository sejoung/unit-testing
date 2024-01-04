# 단위 테스트(생산성과 품질을 위한 단위 테스트 원칙과 패턴)

Rider에 mono를 설치해야 한다.

To run integration tests:

1. Use the script in DatabaseGenerationScript.sql to create the database.
2. Configure the tests to execute sequentially, not in parallel.

```
sudo docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=<YourStrong@Passw0rd>" \
   -p 1433:1433 --name sql1 --hostname sql1 \
   -d \
   mcr.microsoft.com/mssql/server:2022-latest
````

* [단위 테스트(생산성과 품질을 위한 단위 테스트 원칙과 패턴)](http://www.acornpub.co.kr/book/unit-testing)
