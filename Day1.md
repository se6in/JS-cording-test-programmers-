# Day1 

# 두 수의 합
```js
function solution(num1, num2) {
    var answer = num1 + num2;  
    return answer;
}
```
# 두 수의 차
```js
function solution(num1, num2) {
    var answer = 0;
    answer = num1 - num2;
    return answer;
}
```
# 두 수의 곱
```js
function solution(num1, num2) {
    return num1*num2;
}
```
# 몫 구하기
```js
const solution= (num1,num2) => {
        const answer = parseInt(num1 / num2);
        return answer;
}
```
parseInt() - 문자열을 정수로 바꾸는 함수입니다.

# 두 수의 나눗셈
```js
function solution(num1, num2) {
    var answer = parseInt(num1 / num2 * 1000);
    return answer;
}
```
# 숫자 비교하기
```js
function solution(num1, num2) {
    var answer = 0;
    if(num1 == num2){
        answer = 1;
    }
    else if(num1 != num2){
        answer = -1;
    }
    return answer;
}
```
# 분수의 덧셈(틀림)
```js
function fnGCD(a, b){
    return (a%b)? fnGCD(b, a%b) : b;
}

function solution(denum1, num1, denum2, num2) {
    let denum = denum1*num2 + denum2*num1; //분자
    let num = num1 * num2; //분모
    let gcd = fnGCD(denum, num); //최대공약수

    return [denum/gcd, num/gcd];
} 
```
삼항 연산자 - 조건이 참이면 value1 , 거짓이면 value2

(조건) ? value1 : value2 
# 배열 두배 만들기
```js
function solution(numbers) {
    var answer = [];
    
    for(let i = 0; i < numbers.length ; i++){
        answer.push(numbers[i] * 2);
    }
    return answer;
}
```
