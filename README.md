# github-ps calculates a github's project popularity score

[NodeJS](https://github.com/joyent/node) project has been taken as a reference project to evaluate the "normal life" of a project and to estimate relative weight of each criteria (date of these number is 17 april 2012).
  
  - NodeJS pull requests  = 90
  - NodeJS forks = 1681
  - NodeJS tags = 139
  - NodeJS issues = 443+2682
  - NodeJS watchers = 14278
  
Here is the criterias associated to the given weights (relative weight is the first number):

  - Number of pull requests (weight = 150.126 * 3)
  - Number of forks         (weight = 8.4994 * 2)
  - Number of tags          (weight = 102.734 * 2)
  - Number of issues        (weight = 4.58438 * 1)
  - Number of watchers      (weight = 1 * 1)

It has been arbitrary decided that number of pull requests is 3 times heavier than number of watchers. Number of forks are only 2 times heavier than number of watchers.

## Usages examples

```bash
./github-ps node
node project popularity score is 6988
----
score = 6988
pulls = 89
forks = 1681
tags = 139
issues = 3115
open_issues = 432
closed_issues = 2683
watchers = 14280
days_from_start = 1056
no_activity_days = 0
project_url = https://github.com/joyent/node

./github-ps phpfreechat | grep ^score
score = 396

./github-ps github-popularity-score | grep ^score
score = 1
```

## Dependencies

```bash
sudo apt-get install curl wcalc xmllint php5-cli
```
