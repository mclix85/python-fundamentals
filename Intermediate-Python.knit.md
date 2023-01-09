---
title: "Intermediate Python"
subtitle: "Hugo Bowne-Anderson"
date: "02 January 2023"
author:
  - name: "Dat Tran"
output:
  rmdformats::robobook:
    keep_md: true
    thumbnails: true
    lightbox: true
    gallery: true
    use_bookdown: true
---

<style>
body {
  text-align: justify;
}
</style>

<h3><a href="https://github.com/mclix85/main" target="_blank">View Source Code</a></h3>

<h3>Course Description</h3>

<p class="course__description">Learning Python is crucial for any aspiring data science practitioner. Learn to visualize real data with Matplotlib’s functions and get acquainted with data structures such as the dictionary and pandas DataFrame. This four-hour intermediate course will help you to build on your existing Python skills and explore new Python applications and functions that expand your repertoire and help you work more efficiently.
<br><br>
You'll discover how dictionaries offer an alternative to Python lists, and why the pandas dataframe is the most popular way of working with tabular data. In the second chapter of this course, you’ll find out how you can create and manipulate datasets, and how to access them using these structures. Hands-on practice throughout the course will build your confidence in each area.
<br><br>
As you progress, you’ll look at logic, control flow, filtering and loops. These functions work to control decision-making in Python programs and help you to perform more operations with your data, including repeated statements. You’ll finish the course by applying all of your new skills by using hacker statistics to calculate your chances of winning a bet.
<br><br>
Once you’ve completed all of the chapters, you’ll be ready to apply your new skills in your job, new career, or personal project, and be prepared to move onto more advanced Python learning.</p>

# Matplotlib

<p class="chapter__description">
    Data visualization is a key skill for aspiring data scientists. Matplotlib makes it easy to create meaningful and insightful plots. In this chapter, you’ll learn how to build various types of plots, and customize them to be more visually appealing and interpretable.
  </p>

## Basic plots with Matplotlib



### Line plot (1)


<div class>
<p>With matplotlib, you can create a bunch of different plots in Python. The most basic plot is the line plot. A general recipe is given here.</p>
<pre><code>import matplotlib.pyplot as plt
plt.plot(x,y)
plt.show()
</code></pre>
<p>In the video, you already saw how much the world population has grown over the past years. Will it continue to do so? The world bank has estimates of the world population for the years 1950 up to 2100. The years are loaded in your workspace as a list called <code>year</code>, and the corresponding populations as a list called <code>pop</code>.</p>
<p><em>This course touches on a lot of concepts you may have forgotten, so if you ever need a quick refresher, download the <a href="https://datacamp-community-prod.s3.amazonaws.com/0eff0330-e87d-4c34-88d5-73e80cb955f2">Python for data science Cheat Sheet</a> and keep it handy!</em></p>
</div>

<li>
<a href="https://docs.python.org/3/library/functions.html#print"><code>print()</code></a> the last item from both the <code>year</code> and the <code>pop</code> list to see what the predicted population for the year 2100 is. Use two <code>print()</code> functions.</li>

<li>Before you can start, you should import <code>matplotlib.pyplot</code> as <code>plt</code>. <code>pyplot</code> is a sub-package of <code>matplotlib</code>, hence the dot. </li>

<li>Use <a href="https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html"><code>plt.plot()</code></a> to build a line plot. <code>year</code> should be mapped on the horizontal axis, <code>pop</code> on the vertical axis. Don't forget to finish off with the <a href="https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.show.html"><code>plt.show()</code></a> function to actually display the plot.</li>
<div>

```python
# edited/added
import numpy as np
year=list(range(1950,2100+1))
pop=list(np.loadtxt('datasets/Intermediate-Python/pop1.txt', dtype=float))

# Print the last item from years and populations
print(year[-1])
```

```
## 2100
```

```python
print(pop[-1])
```

```
## 10.85
```
</div>

<div>


















































































































































































































