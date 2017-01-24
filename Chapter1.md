
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


* Filter NAN value:
  1. np.isnan(array), produce boolean array
  2. ~booleanArray, reverse element's value
  3. array[~np.isnan(array)] --> filter all nan values in array
  
## Speed of Numpy
* use optimized methods as much as possible!
* array.dot(array) is 25 times faster than np.sum(array * array)
* Use matrix/matrix methods!

## ALL numpy namespace is available in spicy

# Project Part

* sp.genfromtxt("filepath",delimiter = "\t")
* Matrix slice: data[:,0] --> slice to get the all elements that the second dimension is 0.
* Plotting
  * plt.scatter(x,y)
  * plt.title("title")
  * plt.xlabel("xx"),ylabel
  * plt.xticks([w*7*24 for w in range(10)],["week %i"%w for str(w) in range(10)]) --> xticks([numeric array],[label string array])
  * plt.autoscale(tight=True)
  * plt.grid()
  * plt.show()

* polyfit funcs:
  * fitting curves: f1para = sp.polyfit(x,y,polynomial)
  * get the functions from para: f1 = sp.poly1d(f1para)
  * numpy.linspace(start, stop, num=50, endpoint=True, retstep=False, dtype=None) --> get an evenly scattered points from start to stop
  
