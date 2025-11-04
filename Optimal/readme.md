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
