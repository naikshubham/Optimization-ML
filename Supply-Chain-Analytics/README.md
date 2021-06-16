# Supply Chain Analytics in Python

### Basics of Optimization
- Linear Programming (LP) is a Powerful Modeling Tool for Optimization
- It is an optimization method using a mathematical model whose requirements are represented by linear relationships
- There are 3 basic components of LP: 
1. **Decision variables** : or the things that we can control
2. **Objective function** : which describes the goal as a mathematical expression. It is what we want to maximize or minimize, such as profit or costs
3. **Constraints** : Finally, because we live in the real world there are constraints that limit our possible solutions for example manufacturing capicity,
 
#### Example
- Use LP to decide on an excercise routine to burn as many calories as possible in 10 mins

           Pushup            | Running
Minutes | 0.2min per pushup  | 10min per mile
Calories| 3cal per pushup    | 130cal per mile 

- Constraint - only 10 minutes to excercise
- Based on the chart what combination of push-ups and running should we do? Model it as LP problem

#### Basic components of an LP
- **Decision variables** : First, we decide on the decision variables. In this case it is the number of push-ups and miles ran
- **Objective function** : Next, the objective function captures the number of calories burned for each push-up and mile ran. So based on our chart, we add 3 times the number of push-ups to 130 times the number of miles. **Max(3 * number of push-ups + 130 * number of miles) . We want to choose the combination of decision variables that maximizes this function.
- **Constraints** : Finally, we need to express our constraints. (Math expression that describe the limits of a solutions)

##### Constraints 
- 0.2 * Number of Pushups + 10 * Number of miles <=10 : The first constraint captures how many minutes it takes to perform the excercise which must be less than or equal to 10 minutes
- Number of Pushups >= 0 : We also want to ensure our decision variables are not negative
- NUmber of Miles >= 0 

