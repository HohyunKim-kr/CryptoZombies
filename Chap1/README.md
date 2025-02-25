## 3.상태변수 & 정수

'상태 변수' 는 컨트랙트 저장소에 영구 저장됨. 이더리움에 기록됨. 데이테베이스에 쓰는 것과 동일. 


Example)

```solidity
contract Example {
    // 이 변수는 블록체인에 영구적으로 저장됨.
    uint myUsignedInteger = 100;
}
```
### 부호없는 정수: uint
uint 자료형은 부호없는 정수로, 값이 음수가 아님을 의미함.
솔리디티에서 uint는 실제로 uint256, 즉 256비트 부호 없는 정수의 다른 표현. uint8, uint16, uint32 등과 같이 uint를 더 적은 비트로 선언할 수도 있음. 특수한 경우가 아니라면 단순히 uint를 사용.

## 4. 수학 연산
솔리디티의 수학 연산은 기존의 연산과 동일. 
* 덧셈 x + y
* 뺄셈 x - y
* 나눗셈 x / y
* 나머지 x % y

Example)
솔리디티는 지수연산도 지원 
```
uint x = 5 ** 2; // 5^2 = 25
```

## 5. 구조체

string은 임의의 길이를 가진 UTF-8 데이터를 위해 활용.
```solidity
struct Person{
    uint age;
    string name;
}
```

## 6. 배열
어떤 것들의 모음이 필요할 때, 배열을 사용. 정적배열과 동적 배열의 두 종류의 배열이 있음.

```solidity
// 2개의 원소를 담을 수 있는 고정 길이의 배열.
uint[2] fixedArray;
// 동적 배열은 고정된 크기가 없으며 계속 크기가 커짐.
uint[] dynamicArray;
```

구조체 배열
```solidity
Person[]
```