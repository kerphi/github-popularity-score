# github-ps calculates a github's project popularity score

[NodeJS](https://github.com/joyent/node) project has been taken as a reference project to evaluate relative weight of each criteria.

Here is the criterias associated to the given weights (relative weight is the first number):

  - Number of pull requests (weight = 150.126 * 3)
  - Number of forks         (weight = 8.4994 * 2)
  - Number of issues        (weight = 4.58438 * 1)
  - Number of watchers      (weight = 1 * 1)

## Examples

    ./github-ps node
    ./github-ps phpfreechat
    ./github-ps github-popularity-score
    
Should returns someting like that:

    node project popularity score is 5547.21
    phpfreechat project popularity score is 99.3049
    github-popularity-score project popularity score is 1

## Dependencies

    sudo apt-get install curl wcalc xmllint

## Todo

  - Take into account number of tags
  - Take into account time between today and the date of first commit
  - Take into account time between today and the last commit