# 키친포스

## 요구 사항

### 상품

- 상품을 등록할 수 있다.
- 상품의 가격이 올바르지 않으면 등록할 수 없다.
    - 상품의 가격은 0원 이상이어야 한다.
- 상품의 이름이 올바르지 않으면 등록할 수 없다.
    - 상품의 이름에는 비속어가 포함될 수 없다.
- 상품의 가격을 변경할 수 있다.
- 상품의 가격이 올바르지 않으면 변경할 수 없다.
    - 상품의 가격은 0원 이상이어야 한다.
- 상품의 가격이 변경될 때 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 크면 메뉴가 숨겨진다.
- 상품의 목록을 조회할 수 있다.

### 메뉴 그룹

- 메뉴 그룹을 등록할 수 있다.
- 메뉴 그룹의 이름이 올바르지 않으면 등록할 수 없다.
    - 메뉴 그룹의 이름은 비워 둘 수 없다.
- 메뉴 그룹의 목록을 조회할 수 있다.

### 메뉴

- 1 개 이상의 등록된 상품으로 메뉴를 등록할 수 있다.
- 상품이 없으면 등록할 수 없다.
- 메뉴에 속한 상품의 수량은 0 이상이어야 한다.
- 메뉴의 가격이 올바르지 않으면 등록할 수 없다.
    - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴는 특정 메뉴 그룹에 속해야 한다.
- 메뉴의 이름이 올바르지 않으면 등록할 수 없다.
    - 메뉴의 이름에는 비속어가 포함될 수 없다.
- 메뉴의 가격을 변경할 수 있다.
- 메뉴의 가격이 올바르지 않으면 변경할 수 없다.
    - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴를 노출할 수 있다.
- 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 높을 경우 메뉴를 노출할 수 없다.
- 메뉴를 숨길 수 있다.
- 메뉴의 목록을 조회할 수 있다.

### 주문 테이블

- 주문 테이블을 등록할 수 있다.
- 주문 테이블의 이름이 올바르지 않으면 등록할 수 없다.
    - 주문 테이블의 이름은 비워 둘 수 없다.
- 빈 테이블을 해지할 수 있다.
- 빈 테이블로 설정할 수 있다.
- 완료되지 않은 주문이 있는 주문 테이블은 빈 테이블로 설정할 수 없다.
- 방문한 손님 수를 변경할 수 있다.
- 방문한 손님 수가 올바르지 않으면 변경할 수 없다.
    - 방문한 손님 수는 0 이상이어야 한다.
- 빈 테이블은 방문한 손님 수를 변경할 수 없다.
- 주문 테이블의 목록을 조회할 수 있다.

### 주문

- 1개 이상의 등록된 메뉴로 배달 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 포장 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 매장 주문을 등록할 수 있다.
- 주문 유형이 올바르지 않으면 등록할 수 없다.
- 메뉴가 없으면 등록할 수 없다.
- 매장 주문은 주문 항목의 수량이 0 미만일 수 있다.
- 매장 주문을 제외한 주문의 경우 주문 항목의 수량은 0 이상이어야 한다.
- 배달 주소가 올바르지 않으면 배달 주문을 등록할 수 없다.
    - 배달 주소는 비워 둘 수 없다.
- 빈 테이블에는 매장 주문을 등록할 수 없다.
- 숨겨진 메뉴는 주문할 수 없다.
- 주문한 메뉴의 가격은 실제 메뉴 가격과 일치해야 한다.
- 주문을 접수한다.
- 접수 대기 중인 주문만 접수할 수 있다.
- 배달 주문을 접수되면 배달 대행사를 호출한다.
- 주문을 서빙한다.
- 접수된 주문만 서빙할 수 있다.
- 주문을 배달한다.
- 배달 주문만 배달할 수 있다.
- 서빙된 주문만 배달할 수 있다.
- 주문을 배달 완료한다.
- 배달 중인 주문만 배달 완료할 수 있다.
- 주문을 완료한다.
- 배달 주문의 경우 배달 완료된 주문만 완료할 수 있다.
- 포장 및 매장 주문의 경우 서빙된 주문만 완료할 수 있다.
- 주문 테이블의 모든 매장 주문이 완료되면 빈 테이블로 설정한다.
- 완료되지 않은 매장 주문이 있는 주문 테이블은 빈 테이블로 설정하지 않는다.
- 주문 목록을 조회할 수 있다.

## 용어 사전
 
### 상품
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 상품 | Product | 식당에서 판매하는 음식, 음료를 지칭 |
| 이름 | Name | 상품 이름을 지정한다. 비속어는 안된다.  |
| 가격 | Price | 상품의 판매가격. 0원 이상 입력받는다. |
| 등록 | create | 새로운 상품을 등록한다. |
| 가격 변경 | Change Price | 상품의 가격을 변경한다. 0원 이상 입력받는다. |


### 메뉴그룹
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 메뉴 그룹 | Menu Group | 고객에게 보여지는 메뉴그룹 목록이다. ex)한식, 일식, 중식, 점심특가 |
| 이름 | Name | 메뉴 그룹 이름을 지정한다. | 
| 등록 | create | 새로운 메뉴그룹을 등록한다. | 

### 메뉴
| 한글명 | 영문명 | 설명 | 
| --- | --- | --- |
| 메뉴 | Menu | 고객이 보는 메뉴다 |
| 이름 | Name | 메뉴 이름이다. 비속어는 안된다. |
| 가격 | Price | 메뉴의 가격이다. 해당 메뉴에 포함된 상품들의 가격을 초과할 수 없다. |
| 메뉴 상품 | Menu Product | 메뉴에 포함되는 상품이다. |
| 등록 | create | 새로운 메뉴를 등록한다. |
| 공개 | Display | 정상적으로 판매중인 메뉴다. |
| 비공개 | Hide | 모종의 이유(매진)로 메뉴를 숨긴다. |
| 가격 변경 | Change Price | 메뉴의 가격을 변경한다. 0원 이상 입력받는다. 상품들의 가격을 초과할 수 없다. |


### 주문 테이블
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 주문 테이블 | Order Table | 매장 테이블이다. |
| 이름 | Name | 테이블 이름으로 주로 1번, 2번, 3번 형식으로 사용한다. |
| 고객 인원 | Guests | 테이블에 앉는 고객 인원이다. |  
| 자리 안내 | Sit | 고객이 테이블을 배정받고 앉았다. |  
| 테이블 정리 | Clear | 고객이 떠난 테이블을 정리한다. | 
| 인원 변경 | Change Guests | 테이블의 고객 인원을 변경한다. 고객이 있는 테이블만 변경이 가능하다. |


### 주문
| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 주문 | Order | 고객이 메뉴를 주문한다. |
| 유형 | Type | 주문의 유형은 배달, 포장, 매장내 식사로 나눠진다. |
| 상태 | Status | 주문 상황을 표시한다.  <br/>매장내 식사와 포장은 대기 -> 접수 -> 제공 -> 완료로 진행된다.<br/>배달 주문은 대기 -> 접수 -> 제공 -> 배달중 -> 배달됨 -> 완료로 진행한다.|
| 주문 메뉴 | Order Line Item | 주문받은 메뉴 내역이다. |
| 주문 시각 | Order Date Time | 주문이 들어온 시각이다. |
| 배송 주소 | Address | 메뉴를 받을 주소다 |
| 배달 기사 | Rider | 배달 주문을 전달하는 배달 기사를 요청한다. 기사에게 배달 주문 정보(가격, 주소)를 전달한다. |
| 주문 테이블 | Order Table | 주문이 들어온 테이블 번호다. |


## 모델링
