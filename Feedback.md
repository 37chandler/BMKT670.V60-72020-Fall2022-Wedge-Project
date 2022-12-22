## Feedback

Congrats on a new world record for Task 1. I was able to get it under 40 minutes, but that included upload time as well. Nice modular structure with the functions. I probably would have passed in the working directory as well, rather than setting it as a global, but notebooks tend to push people that way. That `pd.Grouper` function is pretty cool. I haven't seen any of the `Pool` stuff before, nor the multithreading.

On Task 2, you have a very efficient implementation. One benefit of doing it in three steps (pulling the cards, taking a random sample, then querying them) is that you can use `random.seed` in Python and get reproducible results. I don't know if that's possible with the SQL version. 

Task 3 looks good and I don't see any meaningful areas of improvement. 


Thanks for your thoughts on improving the project: 

> What would I change? I would maybe break it up into 3 projects, due at points during the semester. I would like to see more data translation and cleanup. Changing values in columns based on other columns, or even adding columns before pushing to GBQ. It would be really fun to start looking at complete orders and trying to match them to recipes. Or do some market basket analysis with the data.

If you split it up, would you have the due dates for Tasks 2 and 3 before Task 1? Or just pace it out? I've thought about doing this and I think it could be a useful way to keep people focused across the course of the semester. Next year the SQL piece is going to get pulled into its own course, so that will free up time to do some of these other analyses. It'd be great to just make a transaction ID so we don't have to keep doing the dumb concatenation stuff. And we could get rid of some of the columns that never get used. There are some others, like `local` and `organic`, which could give rise to their own analyses. Thanks for the thoughts!
