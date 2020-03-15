# Strings

 Anything inside quotes is considered a string in Python, and you can use **single** or **double quotes**:

```python
name1 = "Python Snake" # double quotes
name2 = 'Java Coffee'  # single qutes
print(name1)           # Output: Python Snake 
print(name2)           # Output: Java Coffee
```

Changing the case of the words in a string:

```python
name = "python snake" 
print(name.title())    # Output: Python Snake 
```

Change a string to all uppercase or all lower case letters:

```python
name = "Python Snake"
print(name.upper())    # Output: PYTHON SNAKE
print(name.lower())    # Output: python snake
```

In some situations, you'll want to use a variable's value inside a string:

```python
first_name = "python"
last_name = "snake"
full_name = f"{first_name}{last_name}" # f-strings method, f->format
print(full_name)                       # Output: python snake

message = f"Hello, {full_name.title()}!" 
print(message)                         # Output: Hello, Python Snake!
```

Stripping Whitespace

```python
best_language = " python "
best_language.rstrip()
print(best_language.rstrip())     # Output: " python"

print(best_language.lstrip())     # Output: "python " 
print(best_language.strip())      # Output: "python"
```

