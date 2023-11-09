[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12027493&assignment_repo_type=AssignmentRepo)
# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.

## My Answers
- Three reasons why asymptotic analysis may be misleading
  - We ignore constants, which in practice can make much more difference than we give them credit for
  - $n_0$, smaller inputs can give the appearance of being more efficient than other algorithms but once you get to larger inputs it becomes clear the other algorithm might be more efficient.
  - Excluding when $\Theta$ is used, bounds can be very loose and imprecise
- I believe the program would take 6.667 seconds. I computed this by taking the log of 1,000 which is 3 and the log of 10,000 which is 4, so log 10,000 is roughly $\frac{4}{3}$ of log 1000. So I just multiplied 5 by $\frac{4}{3}$
- There could be any number of reasons that an algorithm would run slower than anticipated:
  - Perhaps the computer it was run on has other things running in the background, slowing it down.
  - Perhaps an error occurred in the IDE and the program didn't run properly behind the scenes.
  - Hardware is not taken into account with asymptotic complexity so maybe the first time it was run was on a modern computer and the second time it was run with the larger input size it was run on a 8-digit basic calculator from the 90s.
