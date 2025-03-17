# This is an h1 header, which is the largest

![Logo of GitHub](https://i.postimg.cc/J4Nsb2PW/github.png)


```py
"""
Implementation of Binary Search Algorithm
"""
def search(nums: list[int], target: int) -> bool:
  """
  Binary Search
  Time Complexity: O(logn)
  Space Complexity: O(1)
  """                                                                                                                             
  n: int = len(nums)                                                                                                                                                    
  l, r = 0, n - 1                                                                                                                                                           
  
  while l <= r:                                                                                                                                                             
    mid: int = (l + r) // 2                                                                                                                                               

    if nums[mid] == target:
       return True                                                                                                                                                       
    elif nums[mid] > target:
       r = mid - 1                                                                                                                                                       
    elif nums[mid] < target:                                                                                                                                              
       l = mid + 1                                                                                                                                                       
         return False                                                                                                                                                          
                                                                                                                                                                                   
     if __name__ == '__main__':                                                                                                                                                
         nums: list[int] = [i for i in range(100)]                                                                                                                             
         for num in [-1, 3, 0, 500, -47, 98, 63, 200]:                                                                                                                         
             target: int = num                                                                                                                                                 
             if search(nums, target):                                                                                                                                          
                 print(f"{target}\t✅ found ")                                                                                                                                
             else:                                                                                                                                                             
                 print(f"{target}\t❌ not found ")
```
