# Study Neural Net

### Example of a Neural Net Mathematical Expression

```python
#input
x = Value(-4.0)
y = Value(2.0)

#intermediate variable
a = x+ y
b= x * y + y**3
a += a + 1
a += 1 + a + (-y)
b += b * 2 + (y + x).relu()
b += 3 * d + (y - x).relu()
c = a - b
d = c**2

#output
z = d / 2.0
z += 10.0 / d

print(f'{z.data:.4f}') # prints 24.7041, the outcome of this forward pass
z.backward()
print(f'{x.grad:.4f}') # prints 138.8338, i.e. the numerical value of dz/dx
print(f'{y.grad:.4f}') # prints 645.5773, i.e. the numerical value of dz/dy
```
