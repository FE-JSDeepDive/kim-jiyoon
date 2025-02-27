## **블록문**

- 블록문(`{}`)은 하나 이상의 문을 그룹화하는 역할
- 단독으로 사용할 수도 있지만, 일반적으로 제어문이나 함수 정의에서 사용됨
- 주의) 블록문 자체는 값을 생성하지 않으며, 자체적으로 유효한 표현식이 아님

## **조건문 (if문, switch문)**

- **if ... else 문**
    - 특정 조건을 평가하여 코드 블록 실행 여부를 결정하는 제어문
    - 조건식은 반드시 불리언(Boolean) 값으로 평가되고,  `true`일 경우 실행됨
    - 주의점)
        
        조건식 내부에서 false로 평가되는 값: `false`, `undefined`, `null`, `0`, `NaN`, `''`(빈 문자열)
        
- **switch 문**
    - 하나의 표현식을 여러 값과 비교할 때 사용됨
    - case 키워드 뒤에 비교할 값이 오며, 일치하는 case 문이 실행됨
    - break 문을 사용하지 않으면 다음 case 문까지 실행이 이어지는 "fall-through(폴스루)" 현상 발생
    - 주의점)
        - 비교 연산은 일치 연산자(`===`) 를 사용 → 자료형까지 일치해야 case 문이 실행됨
        - break를 생략하면 다음 case 문까지 실행될 수 있음

## **반복문 (for, while, do...while)**

- **for 문**
    - 특정 조건이 false가 될 때까지 반복 실행
    - 3개의 식(초기식; 조건식; 증감식)으로 구성
    - 주의점)
        - i < 5가 false가 되는 순간 반복문 종료
        - 반복 횟수가 명확할 때 주로 사용
- **while 문**
    - 조건이 `true`인 동안 계속 실행됨
    - 반복 횟수가 명확하지 않을 때 사용하면 좋음
    - 주의점)
        - 조건이 항상 true → 무한 루프에 빠질 수 있음
- **do...while 문**
    - 반드시 한 번은 실행된 후, 조건이 `true`인 동안 계속 실행됨
    - 차이점)
        - `while` 문은 조건이 false이면 한 번도 실행되지 않을 수 있음
        - `do...while` 문은 조건을 나중에 평가하므로 최소 한 번은 실행됨

## **break 문과 continue 문**

- **break 문**
    - 현재 실행 중인 반복문을 즉시 종료
    - `for`, `while`, `switch`문에서 사용 가능
- **continue 문**
    - 현재 실행을 중단하고 다음 반복을 수행
    - 특정 조건일 때 반복을 건너뛰고 싶을 때 사용
    - 주의점)
        - `continue` 문을 만나면 이후의 코드 실행을 건너뛰고 다음 반복으로 이동
        - `break`와 혼동하지 않도록 주의
