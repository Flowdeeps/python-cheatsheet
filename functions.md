# Python Functions



- [Lambda](#lambda)
- [Declare Function](#lambda)
- [Document Function](#document-function)
- [Get Function Name](#get-function-name)
- [Arguments](#lambda)
- [Decorator](#lambda)
- [Generator](#lambda)
- [Annotation](#lambda)


<br><br>
### Lambda

```python
>>> fn = lambda x: x**3
>>> fn(2)
8

>>> (lambda x: x**3)(2)
9

>>> (lambda x: [x * _ for _ in range(10)])(3)
[0, 3, 6, 9, 12, 15, 18, 21, 24, 27]
```



### Declare Function

```python
def fn_name(): ## Where fn_name represents the function name
    ........
    ........

```


### Get Function Name
```python
## First Declare a function 
def fn_name():
    .......
    .......


>>> fn_name.__name__
'fn_name'
```


### Document a Function
```python
## Document a function with three single quotes
def check():
    '''This function is documented'''
    return


>>> check.__doc__
'This function is documented'
```


### Arguments
```python
>>> def multiply(a, b=0): ## b is 0 by default
...     return a * b
...
>>> multiply(1, 3) ## 3 * 1
3
>>> multiply(5) ## 5 * 0
0
>>> multiply(5, b=3) ## 5 * 3
15
```