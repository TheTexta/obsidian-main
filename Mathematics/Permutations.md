When we have a given number of items and limited positions, where any item can be arranged in any way, and we want to find the number of unique combinations of those items we use [[Factorial|factorials]]. If we have a number of arrangements is *less* then the total number of uniques, then we use the [[nPr formula]] to find the number of arrangements of **n** for **r** spaces. It's important to remember that permutations *counts* possibilities with the same set of uniques in a different position, eg, ABC, BAC, BCA, and ACB are all a unique permutation. Permutations are *not* [[Probability|probabilities]], as permutations *don't* scale for the number of same options which *do* occur multiple times in probabilities. 


### Permutations of indistinguishable objects
While distinct objects can be permutated with the [[nPr formula]], indistinguishable m objects require a unique formula. Find the total options, then find the number of like options n.

$$
\frac{m!}{\sum n!}
$$
