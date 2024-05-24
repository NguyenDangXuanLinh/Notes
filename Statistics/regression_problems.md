# Deal with numberic values, use historical data to predict

## Decision Trees
Overfit -- deep tree with too many leaves
Underfit -- shallow tree little leaves
`max_leaf_nodes=` -- a tree depth to get better performance (avoid underfit overfit)
        
                     __
                  /     \
              leaf1a  leaf1b                
             /  \        /  \
           2a   2b      2c  2d
          / \   / \    / \  / \
         3a 3b 3c 3d  3e 3f 3g 3h

 ## Random Forest
 Uses many (decision) trees -> avg(prediction_of_each_tree) -> can use defult para
