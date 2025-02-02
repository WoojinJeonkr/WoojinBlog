---
layout : post
title : Time complexity and Space complexity
subtitle : 시간복잡도와 공간복잡도에 대해 알아보자
categories : Skill
tags: [Skill, Time_Complexity, Space_Complexity]
---

## 01. 시간 복잡도(Time Complexity)란?
- 입력 길이의 함수로 알고리즘을 실행하는 데 걸리는 시간
- 알고리즘에서 각 코드 명령문을 실행하는 데 걸리는 시간 (알고리즘의 총 실행 시간 x)
- 알고리즘의 연산 횟수(증가 또는 감소)가 발생할 때 실행 시간의 변화(증가 또는 감소)에 대한 정보를 제공한다.
- **알고리즘이 입력 길이의 함수로 실행하는 데 걸리는 시간을 수량화한다.**
  
## 02. 시간 복잡도가 중요한 이유
정의에 따라 알고리즘을 실행하거나 특정 작업을 수행하기 위해 컴퓨터에 제공되어야 하는 일련의 정의된 명령이 필요하다.  
이러한 명령어가 정의되면서 변형이 있을 수 있고 동일한 작업을 수행하기 위해 특정 명령 집합을 정의할 수도 있다. 또한 사용 가능한 프로그래밍 언어 중 하나를 선택할 수 있는 옵션을 통해 명령어는 선택한 프로그래밍 언어의 성능 경계와 함께 모든 형태의 구문을 사용할 수 있다.   
다양한 요소가 실행 중인 알고리즘의 결과에 영향을 미칠 수 있으므로 우리는 이러한 프로그램이 작업을 수행하는 데 얼마나 효율적으로 사용되는지 이해해야 하며 이를 위해서는 알고리즘의 공간 및 시간 복잡도를 모두 고려해야 한다.   

## 03. 시간 복잡도를 계산하는 방법
대표적으로 **Big-O 표기법(빅오 표기법)**이 있다. 우리가 보았듯이 시간 복잡도는 입력 길이의 함수로 시간에 의해 주어지고 시간에 대한 입력 데이터의 크기(n)와 수행된 연산의 수(N) 사이에는 관계가 존재한다. 관계는 시간 복잡도의 증가 순서로 표시되고 O[n] 표기법이 주어진다. (O : 증가 순서, n : 입력의 길이)  

### 001. Big-o 표기법의 유형

```
1. 일정한 시간 - O (1)
2. 선형 시간 – O(n)
3. 대수 시간 – O(log n)
4. 2차 ​​시간 – O(n^2)
5. 세제곱시 – O (n^3)
```

Big-O 표기법에 대해 자세히 알아보려면 <a href="https://www.geeksforgeeks.org/analysis-algorithms-big-o-analysis/" target="_blank" rel="noopener noreferrer" style="color : green">여기</a>를 클릭하세요!

### 002. 알고리즘이 정의되는 과정

1. 차수가 n인 정방 행렬인 2개의 입력 행렬이 주어졌을 때  

2. 두 행렬의 각 요소 값은 np.random 함수를 사용하여 무작위로 선택된다.

3. 처음에 입력 행렬의 차수와 동일한 차수 값이 0인 결과 행렬 할당되고

4. X의 각 요소에 Y의 모든 요소를 ​​곱하고 결과 값을 결과 행렬에 저장한다.

5. 결과 행렬은 목록 유형으로 변환되며 

6. 결과 목록의 모든 요소에 대해 최종 답변을 제공하기 위해 함께 추가된다.

### 003. 정렬 & 검색 알고리즘의 시간복잡도

#### 정렬 알고리즘

- 삽입 정렬
  - 최선: O(n)
  - 최악: O(n^2)
- 병합 정렬
  - 최선, 최악과 상관 없이 O(nlogn)
- 버블 정렬
  - 최선: O(n)
  - 최악: O(n^2)
- 퀵 정렬
  - 최선: O(nlogn)
  - 최악: O(n^2)

#### 검색 알고리즘

- 선형 탐색
  - 최상: O(1)
  - 최악: O(n)
- 이진 검색
  - 최선: O(1)
  - 최악: O(log n)

## 04. 공간 복잡도
시간 복잡도에 대해 들어본 적이 있는 사람이라면 공간 복잡도라는 단어에 대해서도 얼핏 들어본 적이 있을 것이다.   
모든 알고리즘에 필요한 작업 공간 또는 저장소를 공간 복잡도(공간복잡성)이라고 하며 알고리즘이 취하는 입력의 양에 직접적으로 의존하거나 비례한다.   
공간 복잡도를 계산하려면 알고리즘에서 변수가 차지하는 공간을 계산하면 되며 공간이 적을수록 알고리즘이 더 빨리 실행된다.  
참고로 **시간 복잡도와 공간 복잡도는 서로 관련이 없다..**

## 05. 참고 자료
- [What is Time Complexity And Why Is It Essential?](https://www.mygreatlearning.com/blog/why-is-time-complexity-essential/)
- [Time complexity](https://en.wikipedia.org/wiki/Time_complexity)
- [[알고리즘] Time Complexity (시간 복잡도)](https://hanamon.kr/%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98-time-complexity-%EC%8B%9C%EA%B0%84-%EB%B3%B5%EC%9E%A1%EB%8F%84/)
- [Analysis of Algorithms > Big-O analysis](https://www.geeksforgeeks.org/analysis-algorithms-big-o-analysis/)