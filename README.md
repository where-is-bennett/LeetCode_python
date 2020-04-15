# LeetCode_python
LeetCode_python练习和代码都放在这里

测试测试
测试 测试

```python

class Node():
def __init__(self,item):
self.item = item
self.next = None

class Link():
def __init__(self):
self.head = None

def add(self,item):
node = Node(item)
node.next = self.head
self.head = node

def travel(self):
cur = self.head
if cur == None:
print("empty Link")
while cur:
print(cur.item)
cur=cur.next

linkA=Link()
linkA.add(4)
linkA.add(2)
linkA.add(1)
linkA.add(9)
linkA.add(0)
linkA.travel()

linkB=Link()
linkB.add(4)
linkB.add(2)
linkB.add(3)
linkB.travel()

def intersectNode(headA,headB):
cur = headA
s = set()
print("cur2", cur.item)
while cur!=None:
s.add(cur.item)
cur = cur.next
print(s)

cur = headB
print("cur2",cur)
while cur:
if cur.item in s:
print(cur.item)
return
cur =cur.next
intersectNode(linkA.head,linkB.head)
```
