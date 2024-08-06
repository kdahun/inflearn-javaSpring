# JDBC 란?
: Java 기반 애플리케이션의 데이터를 데이터베이스에 저장 및 업데이트하거나, 데이터베이스에 저장된 데이터를 Java에서 사용할 수 있도록 하는 자바 API이다. Java 애플리케이션에서 데이터베이스에 접근하기 위해 JDBC API를 사용하여 데이터베이스에 연동할 수 있으며, 데이터베이스에서 자료를 쿼리하거나 업데이트하는 방법을 제공한다.

![image](https://github.com/user-attachments/assets/b62669e9-3af2-40dc-ad35-d5217a8a2f6f)


- jaga.sql.Connection : 연결
- java.sql.Statement : SQL을 담은 내용
- java.sql.ResultSet : SQL 요청 응답

### JDBC의 동작 흐름

![image](https://github.com/user-attachments/assets/6f303a57-6715-4492-b412-861b7ffbb888)

JDBC는 Java 애플리케이션 내에서 JDBC API를 사용하여 데이터베이스에 접근하는 단순한 구조이다.
JDBC API를 사용하기 위해서는 JDBC 드라이버를 먼저 로딩한 후 데이터베이스와 연결하게 된다.

#### JDBC 드라이버
- 데이터베이스와의 통신을 담당하는 인터페이스
- Oracle, MS SQL, MySQL 등과 같은 데이터베이스에 알맞은 JDBC 드라이버를 구현하여 제공
- JDBC 드라이버의 구현체를 이용하여 특정 벤더의 데이터베이스에 접근할 수 있음.

### JDBC API 사용 흐름

![image](https://github.com/user-attachments/assets/227db407-0a58-4d8a-98ed-8faaa921fe80)

- JDBC 드라이버 로딩 : 사용하고자 하는 JDBC 드라이버를 로딩한다. JDBC 드라이버는 DriverManager 클래스를 통해 로딩된다.
- Connection 객체 생성 : JDBC 드라이버가 정상적으로 로딩되면 DriverManager를 통해 데이터베이스와 연결되는 세션인 Connection 객체를 생성
- Statement 객체 생성 : Statement 객체는 작성된 SQL 쿼리문을 실행하기 위한 객체로 정적 SQL 쿼리 문자열을 입력으로 가진다.
- Query 실생
- 
