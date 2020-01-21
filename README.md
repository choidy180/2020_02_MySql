# MySql

# 소개
+ MySQL은 가장 널리 사용되고 있는 관계형 데이터베이스 관리 시스템(RDBMS: Relational DBMS)<br>
+ MYSQL은 오픈소스, 다중 사용자와 다중 스레드 지원<br>
+ C언어, C++,JAVA, PHP등 여러 프로그래밍 언어를 위한 다양한 API <br>
+ MYSQL은 유닉스, 리눅스, 윈도우 등 다양한 운영체제에서 사용할 수 있으며, 특히 PHP와 함께 웹 개발에 자주 사용<br>
+ MYSQL은 오픈 소스 라이센스를 따르나 상업적으로 사용할 때는 상업용 라이센스 구입필요 <br>

# SQL 기본 <br>
+ DML <br>
  + 데이터 조작 언어<br>
  + 데이터를 조작(선택, 삽입, 수정, 삭제)하는 데 사용되는 언어<br>
  + DML 구문이 사용되는 대상은 테이블의 행 <br>
  + DML 사용하기 위해서는 꼭 그 이전에 테이블이 정의되어 있어야 함 <br>
  + SQL 문 중 SELECT, INSERT, UPDATE, DELETE가 이 구문에 해당<br>
  + 트랜잭션이 발생하는 SQL도 이 DML에 속함<br>
    + 테이블에 데이터를 변경(R/U/D)할 때 실제 테이블에 완전히 적용하지 않고, 임시로 적용<br>
    + 취소가능<br>
    <br>
+ DDL<br>
  + 데이터 정의 언어<br>
  + 데이터베이스, 테이블, 뷰 인덱스 등의 데이터베이스 객체를 생성, 삭제, 변경하는 역할<br>
  + CREATE, DROP, ALTER 구문<br>
  + DDL은 트랜잭션 발생시키지 않음<br>
  + ROLLBACK 이나 COMMIT 사용 불가<br>
  + DDL문은 실행 즉시 MySQL에 적용<br>
  <br>
+ DCL<br>
  + 데이터 제어 언어<br>
  + 사용자에게 어떤 권한을 부여하거나 빼앗을때 주로 사용하는 구문<br>
  + GRANT/REVOKE/<br>
  <br>
  
  + USE<br>
    사용할 테이터 베이스 지정<br>
  + SHOW TABLE<br>
    데이터 베이스에  ??의 테이블 이름 보기<br>
  + SHOW TABLE STATUS<br>
    데이버베이스의 정보 조회<br>
  + DESCRIBE(DESC)<br>
    해당 테이블에 무슨 열이 있는지 확인<br>
    <br>
    
  + SELECT<br>
    + <SELECT... FROM><br>
    + 요구하는 데이터를 가져오는 구문<br>
    + 데이터베이스 내 테이블에서 원하는 정보를 추출<br>
    + SELECT의 구문 형식<br>
      select_expr<br>
      [FROM table_references]<br>
      [WHERE where_condition]<br>
      [GROUP BY {col_name | expr | position}]<br>
      [HAVING where_condition]<br>
      [ORDER BY {col_name | expr | position}]<br><br>
        + SELECT 열이름<br>
          + 테이블에서 필요로 하는 열만 가져오기 가능<br>
          + 여러 개의 열을 가져오고 싶을 때는 콤마로 구분<br>
          + 열이름의 순서는 출력하고 싶은 순서대로 배열가능<br>
+ 기본적인 WHERE절<br>
  + 조회하는 결과에 특정한 조건으로 원하는 데이터만 보고 싶을 때 사용<br>
  + SELECT 필드 이름 FROM 테이블 이름 WHERE 조건 식<br>
  + 조건이 없을 경우 테이블의 크기가 클수록 찾는 시간과 노력이 증가<br>
    ex> SELECT * FROM city WHERE pop >= 8000000; << 인구 800만 이상의 도시만 보여달라는 뜻 <br>
    
+ 관계 연산자의 사용<br>
  + OR , AND , 조건 (=, >, < ...), 관계(NOT , AND , OR 등) 연산자의 조합 가능<br>
  
+ LIKE<br>
  + 문자열의 내용 검색하기 위해 LIKE 연산자 사용<br>
  + 문자 뒤에 %_ 무엇이든 (%) 허용<br>
  + 한 글자와 매치하기 위해서는 _ 사용<br>
  
+ Sub Query<br>
  + 서브쿼리<br>
  + 쿼리문 안에 또 쿼리문이 들어 있는 것<br>
  + 서브 쿼리의 결과가 둘 이상이 되면 에러 발생<br>
  
+ ANY<br>
  + 서브쿼리의 여러 개의 결과 중 한 가지만 만족해도 가능<br>
  + SOME은 ANY와 동일한 의미로 사용<br>
  + =ANY 구문은 IN과 동일한 의미<br>
  
+ ALL<br>
  + 서브쿼리의 여러 개의 결과를 모두 만족 시켜야 함

+ ORDER BY<br>
  + 결과가 출력되는 순서를 조절하는 구문<br>
  + 기본적으로 오름차순 정렬, 내림차순 정렬 - 열 이름뒤에 DESC 적어줄 것<br>
  + ASC(오름차순)은 default 이므로 생략 가능<br>
  

