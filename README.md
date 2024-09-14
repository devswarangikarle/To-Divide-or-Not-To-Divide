# To-Divide-or-Not-To-Divide

def find_number(A, B, N):
    num = (N + A - 1) // A * A
    
    while num % B == 0:
        num += A
    
    return num

T = int(input())

for _ in range(T):
    A, B, N = map(int, input().split())
    result = find_number(A, B, N)
    print(result)
