[Think Stats Chapter 8 Exercise 3](http://greenteapress.com/thinkstats2/html/thinkstats2009.html#toc77)

---

>> The mean error is small and decreases with iterations, so this estimator appears to be unbiased. 

```
def SimulateGame(lam=5, iters=100000):
    """Simulates a game and returns the estimated goal-scoring rate.

    lam: actual goal scoring rate in goals per game
    """
    
    L=[]
    for _ in range(iters):
        goals = 0
        t = 0
        while True:
            time_between_goals = random.expovariate(lam)
            t += time_between_goals
            if t > 1:
                break
            goals += 1
        L.append(goals)

    # estimated goal-scoring rate is the actual number of goals scored
    
    print('Mean Error:', MeanError(L,lam))
    print('RMSE:', RMSE(L,lam))

SimulateGame()
```

---
