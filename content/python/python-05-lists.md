+++
title = "Lists"
slug = "python-05-lists"
weight = 5
+++

A list stores many values in a single structure.

~~~ {.python}
T = [27.3, 27.5, 27.7, 27.5, 27.6]   # array of temperature measurements
print('temperature:', T)
print('length:', len(T))
~~~

~~~ {.python}
print('zeroth item of T is', T[0])
print('fourth item of T is', T[4])
~~~

~~~ {.python}
T[0] = 21.3
print('temperature is now:', T)
~~~

~~~ {.python}
primes = [2, 3, 5]
print('primes is initially', primes)
primes.append(7)   # append at the end
primes.append(11)
print('primes has become', primes)
~~~

~~~ {.python}
print('primes before', primes)
del primes[4]   # remove element #4
print('primes after', primes)
~~~

~~~ {.python}
a = []   # start with an empty list
a.append('Vancouver')
a.append('Toronto')
a.append('Kelowna')
print(a)
~~~

~~~ {.python}
a[99]   # will give an error message (past the end of the array)
a[-1]   # display the last element; what's the other way?
a[:]    # will display all elements
a[1:]   # starting from #1
a[:1]   # ending with but not including #1
~~~

Lists can be heterogeneous and nested:

~~~ {.python}
a = [11, 21, 31]
b = ['Mercury', 'Venus', 'Earth']
c = 'hello'
nestedList = [a, b, c]
print(nestedList)
~~~

You can search inside a list:

~~~ {.python}
'Venus' in b      # returns True
'Mars' in b       # returns False
b.index('Venus')      # returns 1 (position index)
~~~

And you sort lists alphabetically:

~~~ {.python}
b.sort()
b             # returns ['Earth', 'Mercury', 'Venus']
~~~

To delete an item from a list:

~~~ {.python}
b.pop(2)             # you can use its index
b.remove('Earth')       # or you can use its value
~~~

**[Exercise](./solutions/solaa.md):** write a script to find the second largest number in the list [77,9,23,67,73,21].