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
    + SELECT의 구문 형식
      select_expr
      [FROM table_references]
      [WHERE where_condition]
      [GROUP BY {col_name | expr | position}]
      [HAVING where_condition]
      [ORDER BY {col_name | expr | position}]
    
    
    
    
  
