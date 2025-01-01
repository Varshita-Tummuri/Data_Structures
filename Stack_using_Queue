from _collections import deque

class MyStack():

    def __init__(self):
        self.q1=deque()
        self.q2=deque()

    def push(self, x):
        self.q2.append(x)
        while self.q1:
            self.q2.append(self.q1.popleft())
        self.q1, self.q2 = self.q2, self.q1        

    def pop(self):
        if self.q1:
            temp=self.q1[0]
            self.q1.popleft()   
            return temp     

    def top(self):
        if self.q1:
            return self.q1[0]     

    def empty(self):
        if len(self.q1)==0:
            return True
        else:
            return False

obj = MyStack()
obj.push(2)
temp = obj.pop()
print("{temp} is removed")
top = obj.top()
print("{top} is the first element")
param_4 = obj.empty()
print("Is stack empty? Ans:{param_4}")

obj.push(3)
temp1 = obj.pop()
print("{temp1} is removed")
top1 = obj.top()
print("{top1} is the first element")
param_41 = obj.empty()
print("Is stack empty? Ans:{param_41}")

obj.push(10)
temp2 = obj.pop()
print("{temp2} is removed")
top2 = obj.top()
print("{top2} is the first element")
param_42 = obj.empty()
print("Is stack empty? Ans:{param_42}")
