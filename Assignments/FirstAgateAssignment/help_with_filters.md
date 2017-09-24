

```
import warnings
warnings.filterwarnings('ignore')

import agate
```

Let's add some data.


```
salaries = agate.Table.from_csv('Data/nusalaries1718.csv')
```


```
print(salaries)
```

| column                        | data_type |
| ----------------------------- | --------- |
| Employee                      | Text      |
| Position                      | Text      |
| Campus                        | Text      |
| Department                    | Text      |
| Budgeted Annual Salary        | Number    |
| Salary from State Aided Funds | Number    |
| Salary from Other Funds       | Number    |



Now we just want UNL, so we need to filter those out.


```
unl = salaries.where(lambda row: row['Campus'] is 'UNL')
```


```
print(len(unl.rows))
```

    0

Now, what the hell? That should work, right? Well, not exactly. We need to set our row equal to UNL and we can't use the regular `=` to do it. We need to use `==` which in Python is actually equal to. The single equal sign is for assigning variables.


```
unl = salaries.where(lambda row: row['Campus'] == 'UNL')
```


```
print(len(unl.rows))
```

    6315


That's better.
