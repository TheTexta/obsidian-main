When we have a given number of items and limited positions, where any item can be arranged in any way, and we want to find the number of unique combinations of those items we use [[Factorial|factorials]]. If we have a number of arrangements is *less* then the total number of uniques, then we use the [[nPr formula]] to find the number of arrangements of **n** for **r** spaces. It's important to remember that permutations *counts* possibilities with the same set of uniques in a different position, eg, ABC, BAC, BCA, and ACB are all a unique permutation. Permutations are *not* [[Probability|probabilities]], as permutations *don't* scale for the number of same options which *do* occur multiple times in probabilities. 


### Permutations of indistinguishable objects
While distinct objects can be permutated with the [[nPr formula]], indistinguishable m objects require a unique formula. Find the total options, then find the number of like options n.

$$
\frac{m!}{\sum n!}
$$


### Permutations of objects with distinct positions
When you have to find all possible arrangements then you have to find the possible arrangements of that arrangement into given roles you have to be careful. If we have 3 distinct positions and we have to have 2 of 9 seniors and 1 of 5 juniors to fill them what are all the possible combinations? If we just do $9 * 8* 5$ we do get the number of arrangements possible of those three people, but we ignore the distinct positions they can then occupy. do find the number of distinct positions we must take this answer and multiply it by the number of unique positions. **TLDR: Be careful the question doesn't contain sub arrangements in the answer**