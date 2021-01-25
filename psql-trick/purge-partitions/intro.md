# Intro

Very often you have to :

- store large amount of data
- read them (no modification)
- delete them on a given criteria (date, id, flag, text,...)

When you do this with classic tables, you will :

- potentially spend a lot of time to "delete" the data
- face bloat issues
- plan `vacuum` operations which can be complex and lock tables... which is not always possible

In this scenarion, you'll be able to compare different approaches to achieve these goals in a 
very efficient way, with real data.

