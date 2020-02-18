# This is a dummy Markdown file.

**Markdown** formatting is a hanful tool to nicely _format_ the descriptions of your project.

## Lists
### Simply add dashes to create lists

Programming languages I know:
- MATLAB
- Python
- C
- Java (Andoid oriented)
- Visula Studio

### Enumerated lists are made by using numbers + dot [.]
When writing a paper, it's recommended to write the sections in the following order
1. Material and Methods
2. Results (and only results)
3. Introduction
4. Conclusion/Discussion
5. Abstract

### Check lists or to-do lists
Workflow of the next trhee months would be
- [x] Preparing scripts for new round of measurements
- [x] Test the sctipts on research devices
- [ ] Invite subjects for trial measurements
- [ ] If it goes well, perform main measurement round
- [ ] Analyze recorded data
- [ ] Get it written

### Quote your code even language-specificly
#### Shuffling a vector or list

When writing codes in `MATLAB`, use the command `rendperm()` function to suffle the elements of a vector or matrix:
```matlab
% Solution in MATLAB
months = 1:12;
shuffled_months = randperm(months)
% one possible outcome is
shuffled_months = 
3 9 6 12 1 2 5 8 10 7 11 1 4
```

This, however, looks different when you want to do it in `Python`
```python
# First solution in Python: in-place shuffling
import numpy as np
months = np.arange(1, 13)
print('Original months are: ', months)

np.random.shuffle(months)
print('Shuffled months are: ', months)

```
As an alternative, we can use the `random.sample()` function to make a not in-place shuffling:
```python
# Second solution in Python: not in-place shuffling
import random as rnd
months = list(range(1, 13))
print('Original months are: ', months)

shuffled_months = rnd.sample(months, len(months))
print('Shuffled months are: ', shuffled_months)

```






## Tables
Let's assume we want to summarize our recet activities in a table. This would result:

Year | Activity | Detail
------------ | ------------ |------------
2008-2012 | Amirkabir University of Technology | Biomedical Engineering
2012-2014 | University of Tehran | Electrical and Computer Engineering
2014-2016 | Negar Andishgan Company | Research and Development

Command | Description
:--- | :---:
*`ones()`* | creates vector or martix of desired size of all __ones__
*`zeros()`* | creates vector or martix of desired size of all __zeros__







More information can be found here on [Writing on GitHub](https://help.github.com/en/github/writing-on-github)
