# Data-Science

import numpy as np

np.arange(2, 50, 3)

l = []
for i in range(5):
l.append(float(input("Enter 5 numbers:")))
print(l)

arr = np.array(l)
print(arr)
print(type(arr))

l1 = []
for i in range(5):
l1.append(float(input("Enter 5 numbers:")))
print(l1)

arr1 = np.array(l1)
print(arr1)
print(type(arr1))
print(np.concatenate((arr,arr1)))
print(np.sort(np.concatenate((arr,arr1))))

arr = np.array([[[0, 1, 2, 3],
... [4, 5, 6, 7]],
...
... [[0, 1, 2, 3],
... [4, 5, 6, 7]],
...
... [[0 ,1 ,2, 3],
... [4, 5, 6, 7]]])
print(arr.ndim)
print(arr.size)

a = np.array([1, 2, 3, 4, 5, 6])
print(a)
print(a.shape)

a2 = a[np.newaxis, :]
print(a2)
print(a2.shape)

a3 = np.expand_dims(a, axis=0)
print(a3)
print(a3.shape)

a1 = np.array([[1, 1],
[2, 2]])
a2 = np.array([[3, 3],
[4, 4]])
print(a1)
print(a2)
print(np.vstack((a1, a2)))
print(np.hstack((a1, a2)))

a = np.array([11, 11, 12, 13, 14, 15, 16, 17, 12, 13, 11, 14, 18, 19, 20])
print(a)
print(np.unique(a))
unique_values, occurrence_count = np.unique(a, return_counts=True)
print(occurrence_count)

