# 조건문

## 조건문
조건문은 프로그램에서 특정 조건을 평가하고, 그 결과에 따라 실행할 코드 블록을 결정하는 제어 구조이다. 자바스크립트에서 가장 일반적으로 사용되는 조건문은 if, else if, else이다.
<img src="../00_img/조건문.jpg"/>

### if문 
#### 조건문의 역할

- 조건 평가: 주어진 조건이 참인지 거짓인지 평가합니다.
- 코드 흐름 제어: 조건에 따라 다른 코드 블록을 실행하여 프로그램의 흐름을 제어한한다.

#### 주요 구성 요소
1. **`if` 문**: 조건이 참(`true`)일 때 실행되는 코드 블록을 정의한다.
   ```javascript
   if (조건) { // 조건식이란 결과가 참 또는 거짓으로 분류되는 값을 의미함.
       // 조건이 참일 때 실행할 코드
   }
   ```
2. **else if** 문: 추가적인 조건을 평가할 수 있다. 이전 조건이 거짓일 때 다음 조건을 확인한다.
    ```
    else if (조건) {
        // 추가 조건이 참일 때 실행할 코드
    }
    ```

3. **else** 문: 모든 조건이 거짓일 경우 실행되는 코드 블록입니다.

    ```
    else {
        // 모든 조건이 거짓일 때 실행할 코드
    }
    ```


```
// 남편에게 입력된 명령을 프로그램으로 변환한다면

let avocado = true

if(avocado){ // 아보카도가 있다면
    milk = 6;
}else{ // 없다면
    milk = 1;
}
```


### switch문
- `switch` 문은 주어진 표현식의 값을 평가하여 여러 경우(case) 중 하나에 해당하는 코드 블록을 실행하는 제어 구조이니다.
- `switch` 문은 여러 조건을 처리할 때, `if-else` 문보다 가독성이 높고 관리하기 쉬운 경우가 많다.

#### 주요 구성 요소
```javascript
   switch (표현식) {
       case 값1:
           // 값1과 일치할 때 실행할 코드
           break;
       case 값2:
           // 값2와 일치할 때 실행할 코드
           break;
       default:
           // 모든 case와 일치하지 않을 때 실행할 코드
   }
```

1. **`switch` 문**: 평가할 표현식을 지정한다.
2. case: switch 문에서 검사할 각 경우를 정의한다. 각 경우는 case 키워드 다음에 오는 값으로 시작한다.
3. break: 각 case 블록이 실행된 후 switch 문을 종료한다. break가 없으면 다음 case 블록이 계속 실행된다.
4. default: 모든 case와 일치하지 않을 때 실행되는 코드 블록입니다. 선택 사항이다.

---

# 반복문과 흐름 제어

## 개념 설명
반복문은 특정 조건을 만족하는 동안 코드를 반복 실행하는 구조이다. `for`, `while`, `do-while`의 세 가지 주요 반복문이 있다. 각 반복문은 코드 실행 흐름을 제어하며, 반복 횟수나 조건에 따라 다르게 동작한다.

<img src="../00_img/반복문.jpg"/>

### 반복문 종류
- **for문**: 반복 횟수가 명확할 때 사용. 초기화, 조건 검사, 증감 연산을 한 곳에서 처리한다.
- **while문**: 조건이 참인 동안 반복. 조건이 거짓이 되면 종료한다.
- **do-while문**: 최소 한 번은 실행한 후 조건을 검사해 반복 여부를 결정한다.

### 표현식
```js
// for문
for (let i = 0; i < 10; i++) {
    console.log(i);
}

// while문
let i = 0;
while (i < 10) {
    console.log(i);
    i++;
}

// do-while문
let j = 0;
do {
    console.log(j);
    j++;
} while (j < 10);

```