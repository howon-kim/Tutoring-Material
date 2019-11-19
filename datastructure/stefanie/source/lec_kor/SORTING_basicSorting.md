# Sorting l (Basic Sorts)

## Overview
**도치 (Inversion)** : 시퀀스에서 순서대로 배치되어 있지 않은 쌍의 갯수. 도치되어 있지 않는 배열은 정렬되어 있다.

**선택정렬 (Selection Sort)** : 가장 큰 값 혹은 작은 값을 선택함으로서 배열을 정렬하는 방법. 가장 작은 혹은 큰수의 숫자를 정렬되어 있지 않는 배열의 마지막으로 이동한다. 마지막에는 정렬된 배열만이 남게 된다. 이 알고리즘은 기본적으로 기존 배열을 직접 수정한다.

**힙정렬 (Naive Heapsort)** : 모든 값들을 MaxPQ (Max Priority Queue) 에 넣은후, 하나씩 제거 한다. 제일 처음 제거된 아이템은 배열의 가장 마지막으로 이동하게 된다. 그 다음 제거 되는 아이템은 마지막 이전의 위치로 이동하게 된다. 이런식으로 계속 배열을 정렬하게 되면 마지막에는 정렬된 배열만이 남게 된다. 삽입과 삭제의 동작의 효율성은 O(log N) 이고 N 개의 아이템을 삽입하고 삭제한다고 했을때의 효율성은 O(N log N) 이다. 

**삽입정렬 (Insertion Sort)**: 정렬되지 않은 배열의 값을 좌측 정렬된 배열로 서서히 옮기며 정렬하는 방식. 정렬되지 않은 아이템을 좌측의 아이템과 비교하면서 순서를 바꾸는 (swap) 방식. 한번의 swap 은 하나의 도치 (inversion) 을 해결한다.

## Recommended Problems
- Insertion sort 의 best case 와 worst case 는 어떻게 되는가?
	- Best case : $\theta$(N) 
	- Worst case : $\theta$(N^2)

- 배열이 내림차순으로 정렬되어 있다면, 어떤 정렬 알고리즘 (selection sort 혹은 insertion sort) 가 빠른가?
	- Selection sort

