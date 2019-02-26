# c++
隱式類型轉換bug
`vector.size()` is unsigend int
## 發生情況
``` c++
  // vector is empty
  int i = 4;
  if (0 <= i && i <= vector.size() - 1)
    cout << vector.size() << endl;
  cout << i << endl;
```
