# Задача 1. Оценка алгосложности программы
Ниже представлен код на языке `C++`. Ваша задача понять и описать, что он делает, определить его асимптотику (время и дополнительная память) и привести аргументы, почему она именно такая. Результатом выполнения задания должен быть текстовый ответ, написание кода не требуется.

```cpp
int calc(int* arr, int size)
{
  int ans = 0;
  for (int i = 1; i < size; i++)
  {
    ans += arr[i] - arr[i-1];
  }
  return ans;
}
```