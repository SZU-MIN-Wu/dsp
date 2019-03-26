[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

>> In the pregnancy length between first babies and others, the difference in means is 0.029 standard deviations, which is small. However, in the total weight case. The Cohen's effect is -0.089, which means the difference in means is 0.089 standard deviations. The total weight difference between first babies and others has higher effect than pregnancy length.

`python 
print(CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb))`
