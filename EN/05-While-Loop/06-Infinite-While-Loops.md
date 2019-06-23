[slide]
# Infinite Loop
An infinite loop is an instruction sequence that **loops endlessly** when a terminating condition has not been set

An infinite loop is also known as an **endless loop**

# Example: Infinite While Loop (Bug)
```python
command = "Add"
while command != "END": # Always evaluated to True
   print(command)
```

# Example: Finite Loop (Bug Fixed)
```python
command = "Add"
while command != "END":
   print(command)
   command = input()      
```
[/slide]