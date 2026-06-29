# Largest-Number-At-Least-Twice-of-Others
nums=list(map(int,input("Enter the numbers:").split()))
r=max(nums)
c=nums.index(r)
nums.remove(r)
n = len(nums)
for i in range(n):
    if r<2*nums[i]:
        print(-1)
        break
else:
    print(c)
