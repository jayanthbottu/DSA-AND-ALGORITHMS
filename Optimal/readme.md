**Maximum Subarray:**

```
nums = [-1,2,3,-6,2,5,-4]
s,m = 0,0
for n in nums:
    s +=n
    if s<0:
        s=0
    m = max(s,m)
print(m)
```


**Sort an array of 0s 1s 2s**

```
nums = [2,0,1,2,1,0,0,1]
l = m = 0
h = len(nums)-1
for i in range(len(nums)):
    if nums[m]==0:
        nums[l],nums[m]=nums[m],nums[l]
        l+=1
        m+=1
    elif nums[m]==1:
        m+=1
    elif nums[m]==2:
        nums[h],nums[m]=nums[m],nums[h]
        h-=1
print(*nums)
```


**Rotate Image**

```
import numpy as np
matrix = np.array([
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
])
matrix = np.transpose(matrix)
print(matrix[:,::-1])
```



