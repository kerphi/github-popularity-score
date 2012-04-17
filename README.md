# github-ps calculates a github's project popularity score

[NodeJS](https://github.com/joyent/node) project has been taken as a reference project to evaluate the "normal life" of a project and to estimate relative weight of each criteria (date of these number is 17 april 2012).
  - NodeJS pull requests  = 90
  - NodeJS forks = 1681
  - NodeJS issues = 443+2682
  - NodeJS watchers = 14278
  
Here is the criterias associated to the given weights (relative weight is the first number):

  - Number of pull requests (weight = 150.126 * 3)
  - Number of forks         (weight = 8.4994 * 2)
  - Number of issues        (weight = 4.58438 * 1)
  - Number of watchers      (weight = 1 * 1)

It has been arbitrary decided that number of pull requests is 3 times heavier than number of watchers. Number of forks are only 2 times heavier than number of watchers.

## Usages examples

    ./github-ps node
    ./github-ps phpfreechat
    ./github-ps github-popularity-score
    
Should returns something like that:

    node project popularity score is 5547.21
    phpfreechat project popularity score is 99.3049
    github-popularity-score project popularity score is 1

## Dependencies

    sudo apt-get install curl wcalc xmllint

## Todo

  - Take into account number of tags
  - Take into account time between today and the date of first commit
  - Take into account time between today and the last commit