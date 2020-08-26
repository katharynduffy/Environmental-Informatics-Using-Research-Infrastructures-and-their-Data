# Frequently Asked Questions: {-}

## Where can I find due dates for assignments?

*BBLearn*

## How do I know when assignments are due?

*All assignment deadlines can be found in BBLearn.  Within this textbook we have suggestions for the timing of all writen questions, coding labs and final culmination writes ups.  All material by infrastructure is due before we begin the next infrastructure.*

## How do I submit assignments?

*All assignments (except the very first git assignment) are submitted via BBLearn as both .Rmds and .pdfs*

## Do I still have to submit written exercises as .Rmd and .pdf?

*Yes.*

## What's better for code, conciseness or readability?

`Readability > Conciseness`

*I personally almost always use dplyr, my thoughts, pulled largely from Dr. Derek Sonderegger's Statistical Computing Course are below:*

The pipe command in `dplyr` `%>%` allows for very readable code. The idea is that the `%>%` operator works by translating the command *a* `%>%` *f(b)* to the expression *f(a,b)*. This operator works on **any function** and was introduced in the `magrittr` package. The beauty of this comes when you have a suite of functions that take input arguments of the same type as their output.  They are human readable!

For example if we wanted to start with *x*, and first apply function *f()*, then *g()*, and then *h()*, the usual R command would be *h(g(f(x)))* which is hard to read because you have to start reading at the innermost set of parentheses. Using the pipe command `%>%`, this sequence of operations becomes *x* `%>%` *f()* `%>%` *g()* `%>%` *h()*.

Dr. Hadley Wickham (aka R genius) gave the following example of readability:
```
bopping(
  scooping_up(
    hopping_through(foo_foo),
    field_mice),
  head)
```
is more readably written:

```
foo_foo %>% 
  hopping_through(forest) %>%
  scooping_up( field_mice) %>%
  bopping( head )
```

In dplyr, all the functions take a data set as its first argument and outputs an appropriately modified data set. This allows me to chain together commands in a readable fashion.  Then in 3 months I don't have to wonder what on earth I was doing last time I opened this project, if I filtered the data, etc etc.  Your future self will sincerely thank your past self.

## How find I find resources to navigate the NEON Data Portal?

A fantastic powerpoint giving you step-by-step directions [can be found here](https://www.neonscience.org/sites/default/files/Access_NEON_Data_%20Visual_Guide_6Feb2020.pptx).

## How can I best prepare for class and succeed?

1. Read the textbook, click on linked resources including videos, review materials as we go or read ahead.

2. Complete assignments as we go or ahead of time. Do not wait until the last minute.

3. Pick a 'coding buddy' and help each other tackle errors that arise.

4. Reach out to your instructors if you need clarification on assignments.
