## LDA (Linear Discriminant Analysis)


Step of Linear Discriminant
1. Compute Mean of every column for every class in this case ,  the mean will be matrix 3x4 where 3 is class and 4 is column

2. Compute Scatter Within class. The step is below:
   - calculate data points belong to one class minus mean of the class, i will call it A
   - calculate matrix multiplication for A transpose and A
   - add to scatter matrix, do it for all class (SW)

3. Compute scatter between class. the step is below.
   - compute global mean
   - calculate mean of class minus global mean, i will call it B
   - calculate matrix multiplication between B and B transpose, i will call it B'
   - multiply B' with n where n is number of point belong to a class
   - add to scatter matrix, do it for all class (SB)

4. calculate matrix multiplication between SW inverse and SB

5. find eigen for result of number 4

6. sorting eigen from biggest eigen value

7. determine the num_component

8. multiply data point with num_component eigen vector 

feel free to correct it
