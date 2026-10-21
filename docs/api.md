# API 参考

以下接口对应第一部分自动测试实验中的 calculator.py。

## add(a, b)

返回两个数的和。

```python
add(2, 3)  # 5
add(-1, 1)  # 0
```

## multiply(a, b)

返回两个数的积。

```python
multiply(3, 4)  # 12
multiply(2, 0)  # 0
```

## 自动测试

test_calculator.py 使用 pytest 验证以上四条断言。每次推送或提交 Pull Request 时，GitHub Actions 自动运行测试；失败时可从日志定位断言与实际结果的差异。
