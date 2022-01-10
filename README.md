# Queue
A Queue is a linear structure which follows a particular order in which the operations are performed. The order is First In First Out (FIFO).
```python3
class Queue:
    def _init_(self):
        self.items = []

    def is_empty(self):
        return self.items == []

    def enqueue(self, item):
        self.items.insert(0, item)

    def dequeue(self):
        return self.items.pop()

    def print_queue(self):
        print(self.items)

q = Queue()
q.enqueue('a')
q.enqueue('b')
q.enqueue('42')
q.print_queue()

q.dequeue()
q.print_queue()
```
# Stack
Stack is a linear data structure which follows a particular order in which the operations are performed. The order may be LIFO(Last In First Out) or FILO(First In Last Out).
```python3
class Stack:
    def _init_(self):
        self.items = []  
  
    def is_empty(self):
        return self.items == []
  
    def push(self, item):
        self.items.insert(0, item)
    
    def pop(self):
        return self.items.pop(0)
    
    def print_stack(self):
        print(self.items)
    
s = Stack()
s.push('a')
s.push('b')
s.push('c')
s.print_stack()

s.pop()
s.print_stack()
```
