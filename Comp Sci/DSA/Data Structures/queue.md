# Queue
queue is a similer data structure to [[stack]] only difference being its first-in-first-out(**FIFO**) policy. while Inserting an element we insert it from thee beginning.

## operations
1. Insert(enqueueing): pushes an element from the head of the queue 
2. Delete(dequeueing): remove the last element in the queue

```python
class queue:
    def __init__(self) -> None:
        self.Q = []
    def enqueue(self, element):
        self.Q.append(element)
    def dequeue(self):
        self.Q = self.Q[:-1]
    def print(self):
        print(self.Q)

Q = queue()
Q.enqueue(1)
Q.enqueue(2)
Q.enqueue(3)
Q.enqueue(4)
Q.enqueue(5)
Q.print()
Q.dequeue()
Q.print()
```
