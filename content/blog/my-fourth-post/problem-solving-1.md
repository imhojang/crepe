---
title: '[Problem Solving #1] divisibleSumPairs'
date: '2019-05-06 15:54:39'
description: my approach in solving an algorithm called "divisibleSumPairs" using Javascript
---
## 합해서 나눠떨어지는 쌍 찾기 (divisibleSumPairs)

정수로 이루어진 배열 `ar`과 양의 정수 `k`가 있습니다.  
다음과 같은 조건을 만족하는 배열 원소들의 쌍의 개수를 반환하는 함수를 작성해주세요.  
  
(1) `i < j` 이다.  
(2) `ar[i] + ar[j]` 는 `k`의 배수이다.  

예를들어,  
`ar = [1, 2, 3, 4, 5, 6]` 이고 `k = 5` 일때, 조건을 만족하는 쌍은 `[1, 4], [2, 3], [4, 6]` 세 쌍입니다.  
그러므로 결과값은 3이 나와야 합니다.


---
#### 문제 이해 :
  *   **Arguments**  
  (1) `array ar` : an array of integers  
  (2) `integer k` : a positive integer  
  * **Conditions**  
  (1) when `i < j`,  
  (2) and `ar[i] + ar[j]` equal multiples of `k`,  
  (3) `ar[i]` and `ar[j]` are a valid pair
  * **Return**  
  (1) return the number of pairs that meet the condition above.

#### 해결 방법 :  
  * **Create a for loop** that loops through each item in the array (*declare index variable i*)
  * **Create a nested for loop** that always begins one index ahead of the outer loop and loops through rest of the item in the array (*declare index variable j*)
  * **Check if the sum of the integers** at ar[i] and ar[j] are divisible by the *argument integer k*
  * **Count** the number of times the sum of the pairs were multiples of k.  
  * on completion of the loop, **return the count of pairs**

#### 코드 구현 :  
  ~~~
  function divisibleSumPairs(k,ar) {
      var pairCount = 0;
      for (var i = 0; i < ar.length; i++){
          for (var j = i + 1; j < ar.length ; j++) {
              if((ar[i] + ar[j]) % k === 0 ) { pairCount++; }
          }
      }
      return pairCount;
  }  
  ~~~ 

#### 결과 분석 :  
  * **All tests passed !**

    ![fireworks at lotte world tower on May 5th, 2019](fireworksatlotteworldtower.png "The fireworks at Lotte WT")