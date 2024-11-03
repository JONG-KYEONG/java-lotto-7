# java-lotto-precourse

## 기능 요구 사항
- [x] 로또 번호의 숫자 범위는 1~45까지이다.
- [x] 1개의 로또를 발행할 때 중복되지 않는 6개의 숫자를 뽑는다.
- [ ] 당첨 번호 추첨 시 중복되지 않는 숫자 6개와 보너스 번호 1개를 뽑는다.
- [ ] 당첨은 1등부터 5등까지 있다. 당첨 기준과 금액은 아래와 같다.
  -  1등: 6개 번호 일치 / 2,000,000,000원
  -  2등: 5개 번호 + 보너스 번호 일치 / 30,000,000원
  -  3등: 5개 번호 일치 / 1,500,000원
  -  4등: 4개 번호 일치 / 50,000원
  -  5등: 3개 번호 일치 / 5,000원
- [x] 로또 구입 금액을 입력하면 구입 금액에 해당하는 만큼 로또를 발행해야 한다.
- [x] 로또 구입 금액을 입력 받고 해당 금액이 1,000원으로 나누어 떨어지지 않을 경우 예외를 발생시킨다.
- [x] 당첨 번호를 입력받는다.
- [x] 보너스 번호를 입력받는다.
- [x] 보너스 번호가 로또 번호의 범위를 벗어나는 경우 예외를 발생시킨다.
- [x] 사용자가 구매한 로또 번호와 당첨 번호를 비교하여 당첨 내역 및 수익률을 계산한다.
- [ ] 사용자가 잘못된 값을 입력할 경우 IllegalArgumentException을 발생시키고, "[ERROR]"로 시작하는 에러 메시지를 출력 후 그 부분부터 입력을 다시 받는다.
- [ ] Exception이 아닌 IllegalArgumentException, IllegalStateException 등과 같은 명확한 유형을 처리한다.

## 입력 요구 사항
- [ ] 로또 구입 금액을 입력 받는다. 구입 금액은 1,000원 단위로 입력 받으며 1,000원으로 나누어 떨어지지 않는 경우 예외 처리한다.
- [ ] 당첨 번호를 입력 받는다. 번호는 쉼표(,)를 기준으로 구분한다.
- [ ] 보너스 번호를 입력 받는다.

## 출력 요구사항
- [ ] 발행한 로또 수량 및 번호를 출력한다. 로또 번호는 오름차순으로 정렬하여 보여준다.
- [ ] 당첨 내역을 출력한다.
- [ ] 수익률은 소수점 둘째 자리에서 반올림한다. (ex. 100.0%, 51.5%, 1,000,000.0%)
- [ ] 예외 상황 시 에러 문구를 출력해야 한다. 단, 에러 문구는 "[ERROR]"로 시작해야 한다.
