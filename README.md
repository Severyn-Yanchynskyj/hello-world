# hello-world
dvvs
Hanoi towers code(python):

L = [4, 3, 2, 1]
C, R = [], []
def Towers(n, left, cen, right):
    global count
    count += 1  
    if n == 1:
        right.append(left[-1])
        left.pop()
        print(L, C, R)
        return
    Towers(n-1, left, right, cen)

    right.append(left[-1])
    left.pop()
    print(L, C, R)

    Towers(n-1, cen, left, right)

n = 4
print(L, C, R)
count = 0
Towers(4, L, C, R)
print(count)
Add the changes
 
def bubbleSort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(0, n-i-1):
            if arr[j] > arr[j+1] :
                arr[j], arr[j+1] = arr[j+1], arr[j]

