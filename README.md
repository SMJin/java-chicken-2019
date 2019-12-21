# java-chicken-2019
# 우아한 테크코스 2기 최종 오프라인 코딩 테스트 - 치킨집
# 191221 13:10 ~ 18:10

## 기능 구현 목록

### InputView Class
##### Scanner 를 통한 입력이 필요할 때마다 호출할 수 있도록 메소드들을 구현한다.
###### inputPosMenu 메소드 : 첫 메인 화면과 포스기의 원하는 기능을 선택하게 해준다.

### OutputView Class
##### print 문을 통한 출력이 필요할 때마다 호출할 수 있도록 메소드들을 구현한다.
##### printPos 로 먼저 메인 화면을  띄운다.

### Application Class
##### 메인으로 사용되는 클래스로, 처음 printPos 에서 선택한 기능별로 메소드를 따로 구현한다.
##### 주문 등록, 결제하기, 프로그램 종료 를 선택할 수 있게 하는 메소드와, 해당 기능별로 따로 실행을 하게 해주는 세 개의 메소드들을 구현한다.
###### selectPosMenu 메소드 : 첫 메인 화면 포스기의 원하는 기능을 선택하면, 선택한 옵션의 기능을 수행하도록 해준다.
###### selectTable 메소드 : 원하는 테이블을 선택할 수 있게 해주는 출력이 뜨도록 한다.
###### selectOneOption, selectTweOption, selectThreeOption 메소드 : 각 옵션 별로 다르게 실행되도록 한다.

### Table Class
##### 테이블별로 어떤 메뉴를 시켰는지 저장하기 위해서, 총 시킨 음식 가격 등의 필드를 만든다.
##### 99개 이상의 메뉴는 시킬 수 없으므로, 메뉴 수에 대한 것도 구현한다.
##### 메뉴와 해당 메뉴의 수량, 금액을 저장하도록 한다.

### Discount Class
##### 음식의 수량과 어떤 유형으로 결제를 했는지 받아서 할인율을 계산해서 최종 결제할 금액을 출력한다.

## -- 예외처리 exception
### PosNumber Class
##### 처음 메인 화면 포스기의 옵션을 선택할 때 사용되는 숫자들의 예외처리를 해주는 클래스이다.
###### 생성자에서 예외처리를 해준다.
###### isOptionOne, isOptionTwo, isOptionThree 메소드 : 각 해당하는 옵션을 선택했는지 확인해주는 메소드들이다.