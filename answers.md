# Big O Answers

## Snippet 1 -

### Big O:

### Explanation: O(n) because the as data grows the loop iteration grows.

```python
def largest(array, value):
  for item in array:
    if item > value:
      return False
  return True
```

## Snippet 2 -

### Big O:

### Explanation: O(2n) because it loops through the data twice but not in a nested loop

```python
def info_dump(customers):

  print('Customer Names:')
  for customer in customers:
    print(customer['name'])

  print('Customer Locations:')
  for customer in customers:
    print(customer['country'])

```

## Snippet 3 -

### Big O:

### Explanation: O(1) because the function only looks at the first value in the data and returns True or False if matched with the value.

```python
def first_element_is_red(array):
  return array[0] == 'red'
```

## Snippet 4 -

### Big O:

### Explanation: O(n^2) because we loop through O(n) with a nested O(n)

```python
def duplicates(array):
  for index1, item1 in enumerate(array):
    for index2, item2 in enumerate(array):
      if index1 == index2:
        continue
      if item1 == item2:
        return True
  return False
```

## Snippet 5 -

### Big O:

### Explanation: O(n \* m) because we loop O(n) with a O(m) nested inside.

```python
words = ['chocolate', 'coconut', 'rainbow']
endings = ['cookie', 'pie', 'waffle']

for word in words:
  for ending in endings:
    print(word + ending)

```

## Snippet 6 -

### Big O:

### Explanation: O(n) because it has one loop and it grows as the data grows

```python
numbers = [1,2,3,4,5,6,7,8,9,10]

def print_array(array):
  for item in array:
    print(item)

```

## Snippet 7 -

### Big O:

### Explanation: O(n^2) because the nested while inside the for loop is looping through the same data but with certain parameters from the for loop

```python
# this is insertion sort
def insertionSort(arr):
  for i in range(1, len(arr)):
    key = arr[i]
    j = i-1
    while j >=0 and key < arr[j] :
      arr[j+1] = arr[j]
      j -= 1
    arr[j+1] = key
```

## Snippet 8 -

### Big O:

### Explanation: O(n^2) because the nested loop loops through the same data as the primary loop.

```python
for i in range(len(my_list)):
  min_idx = i
  for j in range(i+1, len(my_list)):
      if my_list[min_idx] > my_list[j]:
          min_idx = j

  my_list[i], my_list[min_idx] = my_list[min_idx], my_list[i]
```
