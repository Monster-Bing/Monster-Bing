### 这是一个运用切片法求解轮转问题
\```
    nums = [1, 2, 3, 4, 5, 6, 7]
    k = 3
    a = nums[-k:]
    b = nums[:-k]
    print("{}\n{}".format(a, b))
    nums[:] = a + b
    print(nums)
\```
\
---
