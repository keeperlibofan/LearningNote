### leetcode 

平均每天1.3道题
一周要刷10道题目

- 8月23日
  - findPeakElement, searchRange

```
1. A[mid] > A[mid + 1] && A[mid] > A[mid - 1]，那么，根据定义，mid指向的就是一个峰值

2. A[mid] < A[mid + 1]，因为A[n - 2] > A[n - 1]，那么，一定有一个峰值存在于[mid + 1, n - 2]

3. A[mid] < A[mid - 1]，因为A[0] < A[1]，那么，一定有一个峰值存在于[1, mid - 1]
```

- 8月22日
  - findKthLargest, topKFrequent

- 8月21日
  - \<nil\>

- 8月20日
  - topKFrequent

- 8月19日
  - sortColors, exsits