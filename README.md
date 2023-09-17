# Writing good documentation

## Step 1 - Using codeblocks

codeblocks in markdown make it *very easy* for techies to **copy, paste, share** code.
A good _cloud engineer_ uses codeblocks whenever possible

Because it allows others to copy and paste their code to replicate or research issues.


- In order to create code blocks in markdown you need to use backticks(`)

```
import math

def binomial_distribution(n, k, p):
    """
    Calculate binomial distribution.

    Parameters:
    n (int): number of trials
    k (int): number of successful trials
    p (float): probability of success on each trial

    Returns:
    float: probability of getting exactly k successes in n trials
    """
    # calculate combination of n choose k
    comb = math.comb(n, k)

    # calculate probability
    prob = comb * (p ** k) * ((1 - p) ** (n - k))

    return prob

# example usage:
n = 10  # number of trials
k = 5   # number of successful trials
p = 0.5 # probability of success on each trial

print(binomial_distribution(n, k, p))
```

- When you can, apply syntax highlighting to your code blocks
  
```py
import math

def binomial_distribution(n, k, p):
    """
    Calculate binomial distribution.

    Parameters:
    n (int): number of trials
    k (int): number of successful trials
    p (float): probability of success on each trial

    Returns:
    float: probability of getting exactly k successes in n trials
    """
    # calculate combination of n choose k
    comb = math.comb(n, k)

    # calculate probability
    prob = comb * (p ** k) * ((1 - p) ** (n - k))

    return prob

# example usage:
n = 10  # number of trials
k = 5   # number of successful trials
p = 0.5 # probability of success on each trial

print(binomial_distribution(n, k, p))
```

