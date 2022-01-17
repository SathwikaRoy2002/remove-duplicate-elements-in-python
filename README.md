# remove-duplicate-elements-in-python
list = []
n = int(input("enter a number of elements"))
for i in range(0,n):
    ele = int(input())
    list.append(ele)
    
removeEle = []
m = int(input("enter number of elements to be removed"))
for i in range(0,m):
    ele = int(input())
    removeEle.append(ele)

print("original list", list)
print("elements to be removed : ", removeEle)
list = [ele for ele in list if ele not in removeEle]
print(list)
