# Stack
Stack is a dynamic set in which elements are Deleted by pop operation and Inserted by Push operation.
stack impliment last-in-first-out(**LIFO**) policy.

## operations
1. PUSH: it adds an element in the stack
2. POP: removes top element of the stack
3. EMPTY: returns True if stack is empty else False

## implementation
```python
class Stack:
    def __init__(self):
        self.stack = []
    
    def push(self, element):
        self.stack.append(element)

    def pop(self):
        self.stack = self.stack[1:]

    def is_empty(self) -> bool:
        return True if len(self.stack) == 0 else False

    def print(self):
        print(self.stack)

stack = Stack()
print(stack.is_empty())
stack.push(1)
stack.push(2)
stack.push(3)
stack.push(4)
stack.print()
stack.pop()
stack.print()
print(stack.is_empty())
```
### result:
```
True
[1, 2, 3, 4]
[1, 2, 3]
False
```
