# Data Science Challenge

### Question 1
There is a laundry bin with 20% blue socks.
You randomly draw 10.
What is the probability that 2 are blue?

### Question 2
Out of a set of 1000 emails, 700 are spam.
400 of the emails have the word "free"; 300 of those are spam.
100 of the emails have the word "credit"; 90 of those are spam.
You get an email that contains both "free" and "credit".
What is the probability it is spam?

### Question 3
Using `scatter.csv`: how do you interpret the linear regression?

### Question 4
Using `scatter.csv`: Plot a histogram of the x values.

### Question 5
SQL: There are two tables.
One table contains a list of tests and the other contains the positive results of the tests.
Positives and tests are matched by their ID.
There is at most one positive matching to a test.

Tables:
```
test:
	column: name = 'id', type = int
	column: name = timestamp, type = timestamp
	
positive:
	column: name = 'id', type = int
```
Write an SQL query that shows the daily positive rate.

Example output of your query would look something like:
```
| date       | rate |
----------------------
| 2022-01-01 | 0.23 |
| 2022-01-02 | 0.33 |
... etc.
```

### Challenge 6
Train a prediction model with `train.csv` using the final column as the labels.
Use this model to create labels for the entries in `test.csv`.
Though the labels in `train.csv` are 0/1, the labels created for `test.csv` can be continuous [0 to 1].
Output should be a file called `labels.txt`.
Each line of `labels.txt` is a predicted label for the corresponding line in `test.csv`.
For example, `labels.txt` line 6 will be the predicted label for line 6 in `test.csv`.
The contents of `labels.txt` will look something like:
```bash
0.5355877
0.128361
0.2841359
0.4216329
...etc
```
The quality of the predictions will be judged by RMSE.
Please include the source code used to create your model as well as a write-up of your technique.

