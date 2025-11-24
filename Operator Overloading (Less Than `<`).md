# 🐍 Python OOP: Operator Overloading (Less Than `<`)

## 🎯 AIM

To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.

---

## 🧠 ALGORITHM

1. **Create Class `A`**:
   - Define the `__init__()` method to initialize the object with a value `a`.

2. **Overload the `<` Operator**:
   - Define the `__lt__()` method with logic:
     - If `self.a < o.a`, return `"ob1 is less than ob2"`
     - Else, return `"ob2 is less than ob1"`

3. **Create Objects**:
   - Instantiate two objects `ob1` and `ob2` with values.

4. **Use `<` Operator**:
   - Use `print(ob1 < ob2)` to trigger the overloaded behavior.

---

## 💻 Program:
```
class A:
      def __init__(self,value):
          self.value=value
      def __lt__(self,other):
          if isinstance(other,A):
              return self.value<other.value
          return NotImplemented
  ob1=A(20)
  ob2=A(10)
  if ob2<ob1:
      print("ob2 is less than ob1")
  else:
      print("ob1 is less than ob2")
```
## Output:

![503985405-fd35e148-e435-4a94-b005-a36c745669d4](https://github.com/user-attachments/assets/d9c4b496-1bee-47e2-b401-caccf16aab51)

## Result:
   Thus, the program has executed successfully.
