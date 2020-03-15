---
description: A list is a collection of items in a particular order.
---

# Lists

You can put anything you want into a list, and the items in your list don't have to be related in any particular way. Because a list usually contains more than one element, it's good idea to make the name of your list plural.

```python
fruits = ['apple', 'banana', 'orange', 'peach']
print(fruits)            # Output: ['apple', 'banana', 'orange', 'peach']
```

To access elements in a list

```python
fruits = ['apple', 'banana', 'orange', 'peach']
print(fruits[0])         # Output: apple
```

Python has a special syntax for accessing the last element in a list. Python always returns the last item in the list by asking for the item at index -1:

```python
fruits = ['apple', 'banana', 'orange', 'peach']
print(fruits[-1])        # Output: peach 
print(fruits[-2])        # Output: orange
print(fruits[-3])        # Output: banana
print(fruits[-4])        # Output: banana
```

Changing, Adding, Removing Elements

```python
#Changing#
fruits = ['apple', 'banana', 'orange', 'peach']
fruits[0] = 'kiwi'
print(fruits)             # Output: ['kiwi', 'banana', 'orange', 'peach']

#Adding#
fruits.append('pineapple')
print(fruits)             # Output: ['kiwi', 'banana', 'orange', 'peach', 'pineapple']

fruits.insert(0,'watermelon')
print(fruits)             # Output: ['watermelon', 'kiwi', 'banana', 'orange', 'peach', 'pineapple']

#Removing#
del fruits[1]     
print(fruits)             # Output: ['watermelon', 'banana', 'orange', 'peach', 'pineapple']

popped_lastfruit = fruits.pop()
popped_firstfruit = fruits.pop(0)
print(fruits)             #Output: ['banana', 'orange', 'peach']
print(popped_lastfruit)   #Output: pineapple
print(popped_firstfruit)  #Output: watermelon

fruits.remove('orange')
print(fruits)             #Output: ['banana', 'peach']
 
```

{% hint style="warning" %}
You can no longer access the value that was removed from the list after the del statement is used.
{% endhint %}

{% hint style="warning" %}
Remember that each time you use pop\(\), the item you work with is no longer stored in the list. However, pop\(\) method allow you to store the value to a variable before removing it from a list.
{% endhint %}

{% hint style="warning" %}
The remove\(\) method deletes only the first occurrence of the value you specify. If there's a possibility the value appears more than once in the list, you'll then need to use a loop to make sure all occurrences of the value are removed. - Will be learn in Chapter 7 
{% endhint %}

Organising a list

```python
cars = ['bmw', 'audi', 'toyota', 'subaru']
cars.sort()                # sorted in alphabetical order
print(cars)                # Output: ['audi', 'bmw', 'subara', 'toyota']

cars.sort(reverse=True)    # sorted in reverse alphabetical order
print(cars)                # Output: ['toyota', 'subara', 'bmw', 'audi']
```

{% hint style="warning" %}
After a list is sorted with sort\(\), we can never revert to the original order.
{% endhint %}

To maintain the original order of a list but present it in a sorted order:

```python
cars = ['bmw', 'audi', 'toyota', 'subaru']
print(sorted(cars))        # Output: ['audi', 'bmw', 'subara', 'toyota']
print(cars)                # Output: ['bmw', 'audi', 'toyota', 'subaru']
```

Printing a list in reverse order

```python
cars = ['bmw', 'audi', 'toyota', 'subaru']
cars.reverse()             # Change the order of a list permanently
print(cars)                # Output: ['subaru', toyota, 'audi', 'bmw']
```

Finding the length of a list:

```python
cars = ['bmw', 'audi', 'toyota', 'subaru']
print(len(cars))           # Output: 4
```

