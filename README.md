c, v = map(int,input().split())
votes = list(map(int,input().split()))
base = {}
for vote in votes:
    base[vote] = base.get(vote,0) + 1
if max(base.values()) > c//2:
    print('YES')
else:
    print('NO')