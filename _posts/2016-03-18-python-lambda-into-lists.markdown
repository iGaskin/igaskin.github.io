---
layout: post
title:  "Reversing a number into a list"
---
Leveraging the power of the `lambda` function, we can apply a "headless function" to an iterable item. Lets look at this simple example:
> Given a non-negative integer, return an array containing a list of independent digits in reverse order.


{% highlight python %}
def digitize(n):
    n = str(n)[::-1]
    return map(lambda x: int(x), [x for x in n])
{% endhighlight %}

Our utilization of the lambda function, in conjunction with some python list expansion, has circumvented the need for other more complex looping mechanisms.  Although `lambda` functions may seem scare in practice, they are useful to have in your tool-belt to craft a more elegant solution to a problem.
