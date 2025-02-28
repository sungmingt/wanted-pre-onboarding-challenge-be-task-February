1. 관계형 데이터베이스(RDBMS)와 비관계형 데이터베이스(NoSQL)의 장단점 비교

- RDB는 테이블들이 복합적으로 연관되어 있기 때문에 스키마 변경이 어렵고, 이로 인해 scale out에 용이하지 못힌 반면, NoSQL은 scale out에 용이합니다. 
- RDB는 데이터 무결성이 보장되고, 스키마가 명확하기 때문에 이 데이터 구조를 이용하여 복잡한 의사결정을 할 수 있는 반면, 데이터 구조가 명확하지 않은 NoSQL의 경우 간단한 데이터의 입출력에 적합합니다.
- RDB는 데이터 무결성과 정합성을 위해 트랜잭션과 같은 다양한 기능을 지원하는 반면, NoSQL은 트랜잭션 지원이 없는 경우가 많습니다.


2. 트랜잭션(transaction)이란 무엇인가요?

- 트랜잭션이란 데이터베이스에서 하나의 논리적 작업 단위를 뜻합니다. 
트랜잭션은 여러개의 동작(읽기, 쓰기 등...)들로 이루어질 수 있으며, 트랜잭션의 결과는 commit 또는 rollback입니다.


3. MySQL에서 조인(join)의 역할은 무엇인가요? 다양한 join의 방식에 대해 설명해주세요.

- join이란 RDB에서 두 개 이상의 테이블들을 특정 column을 매개로 조합하여 조회하는 방식이며, 주로 where절과 함께 사용됩니다. 
- join의 종류로는 inner join, outer join(left, right, full) 등이 있습니다.


4. MySQL에서 인덱스(index)란 무엇인가요?

- index란 테이블의 조회 성능 향상을 목적으로 사용되며, 주로 B-tree 또는 B+tree 알고리즘을 통해 구현됩니다.
- 기존의 full scan 방식은 데이터가 늘어날수록 비효율적인 반면, index를 사용하면 일정한 읽기 속도를 보장해줍니다.
- 하지만 데이터의 수정 또는 삭제가 빈번히 일어나는 경우 indexing을 위해 다시 정렬되어야 하므로, 상황에 따라 알맞게 사용해야 합니다.
