# 📚 SQL 학습 리포지토리 (korit_07_sql)

## 🎯 개요
SQL 기초부터 고급 데이터 조작 기법까지 체계적으로 학습한 기록을 적어둔 자료입니다.

## 📖 학습 진행 순서

### 1️⃣ 기초 단계 - RDBMS 기본 개념
- **SELECT, FROM, WHERE, ORDER BY** 기본 쿼리 구조 `korit_07_sql:141-167`
- 데이터 필터링 및 정렬 기법 `korit_07_sql:228-363` 
- SQL 실행 순서 이해 `korit_07_sql:318-333` 

### 2️⃣ 중급 단계 - 데이터 집계 및 그룹화
- **집계 함수**: COUNT, SUM, AVG, MIN, MAX `korit_07_sql:19-30` 
- **GROUP BY**를 활용한 그룹별 계산 `korit_07_sql:133-154` 
- **HAVING**을 통한 집계 결과 필터링 `korit_07_sql:265-317` 

### 3️⃣ 고급 단계 - 복합 데이터 조작
- **JOIN 연산**: INNER, LEFT, RIGHT, CROSS JOIN `korit_07_sql:41-78` 
- **UNION 연산**: 데이터 수직 결합 `korit_07_sql:129-199` 
- **서브쿼리**: 스칼라, 인라인 뷰 `korit_07_sql:200-270` 

### 4️⃣ 실무 단계 - 데이터베이스 관리
- **DDL**: 데이터베이스/테이블 생성 및 수정 `korit_07_sql:1-65` 
- **DML**: 데이터 삽입, 수정, 삭제 `korit_07_sql:67-90` 
- **외래키 관계** 및 복합 기본키 설정 `korit_07_sql:165-180` 

## 🗃️ 샘플 데이터베이스 구조

### 📊 E-commerce 스키마
- **users**: 회원 정보 (id, username, phone, city, country, 마케팅 동의 등)
- **staff**: 직원 정보 (id, user_id, 성명, 생년월일)
- **orders**: 주문 정보 (id, user_id, staff_id, 주문일자)
- **products**: 제품 정보 (id, name, price, discount_price)
- **orderdetails**: 주문 상세 (id, order_id, product_id, quantity)

## 💡 주요 학습 내용

### 🔍 기본 쿼리 패턴
```sql
SELECT column_list
FROM table_name  
WHERE filtering_conditions
ORDER BY sorting_criteria;
```

### 🔗 고급 JOIN 예제
다중 테이블 결합을 통한 복합 데이터 조회 `korit_07_sql:1-10` 

### 📈 서브쿼리 활용
계산된 컬럼 추가 및 조건부 데이터 필터링 `korit_07_sql:209-220` 

## 🚀 시작하기

1. **기초 개념 학습**: RDBMS 원리 및 기본 SQL 문법
2. **핵심 연산 실습**: SELECT, WHERE, ORDER BY 연산
3. **샘플 데이터 로드**: CSV 파일들을 데이터베이스에 임포트
4. **고급 기법 학습**: JOIN, UNION, 서브쿼리 순서로 진행
5. **스키마 설계**: 엔터티 관계 및 정규화 원칙 적용

## 📁 파일 구조
- `learning_logs/20250915.md`: SQL 기초 문법
- `learning_logs/20250916.md`: 집계 함수 및 GROUP BY
- `learning_logs/20250917.md`: JOIN, UNION, 서브쿼리
- `learning_logs/20250918.md`: DDL/DML 및 데이터베이스 설계
- `*.csv`: 실습용 샘플 데이터

## Notes

이 리포지토리는 실무 중심의 SQL 학습을 위해 설계되었으며, 각 단계별로 실제 업무에서 자주 사용되는 쿼리 패턴들을 다룹니다 <cite/>. 정규화된 데이터베이스 구조를 통해 관계형 데이터베이스의 핵심 개념을 실습할 수 있도록 구성되어 있습니다 <cite/>.
