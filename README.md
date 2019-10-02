# Kanhaiya
def IsSorted(lst): 
 
    flag = 0
    i = 1
    while i < len(lst): 
        if(lst[i] < lst[i - 1]): 
            flag = 1
        i += 1
          

    return flag

lst=[1,2,3,4,5]

        
def bubbleSort(arr):
    n = len(arr)
    for i in range(n):
 
        for j in range(0, n-i-1):
 
           if arr[j] > arr[j+1] :
                arr[j], arr[j+1] = arr[j+1], arr[j]

try:
    assert IsSorted(lst) == 0
    print("List is sorted")

except:
    print("List is not sorted")

