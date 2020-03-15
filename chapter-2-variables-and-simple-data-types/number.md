# Number

Python uses two multiplication symbols to represent exponents:

```python
>>> 3 ** 2    // 3^2
9
```

When divide any two numbers, even if they are integers that result in a whole number, you'll always get a float:

```python
>>> 4/2    
2.0

>>> 1 + 2.0
3.0
```

{% hint style="success" %}
Python defaults to a float in any operation that uses a float, even if the output is a whole number.
{% endhint %}

When you're writing long numbers, you can group digits using underscores to make large numbers more readable:

```python
universe_age = 14_000_000_000
print(universe_age) // Output: 14000000000
```

{% hint style="success" %}
To Python, 1000 = 1\_000 = 10\_00
{% endhint %}

