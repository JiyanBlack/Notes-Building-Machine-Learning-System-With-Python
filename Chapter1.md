
# Numpy

* np.array([1,2,3])
* array.ndim -> n dimension
* array.shape -> the shape of a array

* b = array.reshape((3,2)) --> change an array to an 3x2 matrix
* c = a.reshape((3,2)).copy()

## Array/Matrix Manipulation
* a*2, a**2 --> for individual element
* Array Indexing: 
  1. a[ap.array([2,3,4])] --> get 2,3,4th element into a new array.
  2. a[[True,False,True...]] --> boolean index
  3. a>4 --> produce boolean index [True, False, True...]
  4. combined: a[a>4]
  5. support assignment: a[a>4] = 4, trim the outrages, same as a.clip(0,4)
