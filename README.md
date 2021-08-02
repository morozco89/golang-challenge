# First Todo: Enabling cache

The first thought that crossed my mind when I looked at the code was that there was no way to keep track of each price "age".

Then I realize maybe map[string]float64 was not the right data structure to represent the cache.

So I created a type (struct CachedPrice) to model the price and the time at which that price was retrieved from actual service.

This time will help me to compare against TransparentCache configured maxAge and determinate weather or not that price was still valid. 

# Golang-Challenge
Challenge test

We ask that you complete the following challenge to evaluate your development skills.

## The Challenge
Finish the implementation of the provided Transparent Cache package.

## Show your work

1.  Create a **Private** repository and share it with the recruiter ( please dont make a pull request, clone the private repository and create a new private one on your profile)
2.  Commit each step of your process so we can follow your thought process.
3.  Give your interviewer access to the private repo

## What to build
Take a look at the current TransparentCache implementation.

You'll see some "TODO" items in the project for features that are still missing.

The solution can be implemented either in Golang or Java ( but you must be able to read code in Golang to realize the exercise ) 

Also, you'll see that some of the provided tests are failing because of that.

The following is expected for solving the challenge:
* Design and implement the missing features in the cache
* Make the failing tests pass, trying to make none (or minimal) changes to them
* Add more tests if needed to show that your implementation really works
 
## Deliverables we expect:
* Your code in a private Github repo
* README file with the decisions taken and important notes

## Time Spent
You need to fully complete the challenge. We suggest not spending more than 3 days total. Please make commits as often as possible so we can see the time you spent and please do not make one commit. We will evaluate the code and time spent.
 
What we want to see is how well you handle yourself given the time you spend on the problem, how you think, and how you prioritize when time is insufficient to solve everything.

Please email your solution as soon as you have completed the challenge or the time is up.
