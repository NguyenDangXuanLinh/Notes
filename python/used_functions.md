# Loop, Def and Functions, Method

## Store best values of a dictionary using key(s)
`.get` -- get value of the key 'name'  -> val = score.get(4)
`max(val, key=val.get)` -- iterate each key to get value, then compare until max

## Dict comprehensions
Create / change to / tranform dictionaries

Basic syntax -- name= {key: value for key, value in item}
### Create with **iteam iterable**
-  if condi --
  
        `even_squares = {x: x**2 for x in range(1, 11) if x % 2 == 0}`

-  a loop --

        `leaf_nodes = [5, 25, 50, 100, 250, 500]
         score = {leaf_size: get_mae(leaf_size, train_X, val_X, train_y, val_y) \
         for leaf_size in leaf_nodes} `

         
- Change from lists of tuple
  
        pairs = [('a', 1), ('b', 2), ('c', 3)]
        pair_dict = {key: value for key, value in pairs}
  
- Tranform existing dict : swaps the keys and values of ori_dict
  
      ori_dict = {'a': 1, 'b': 2, 'c': 3}
      swap_dict = {value: key for key, value in ori_dict.items()}

  **Note**:
    - `value: key` -- swaps keys and values
    - `.items()` -- returns key-value pairs of ori
    
