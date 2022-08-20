# Linear-Regression-on-EEG-

This analysis was performed on the Kiloword dataset, which had 75 participants perform a go/no go lexical decision task involving 960 English words. They were hooked up to EEG cap with 29 electrodes as they performed the task. The dataset contains detailed metadata with the following characteristics of each word presented: number of letters, concreteness, word frequency, orthographic distance, consonant to vowel proportion, visual complexity, and bigram frequency.   

I used the metadata to create a multiple linear regression to estimate relationships between word attributes and ERPs using Python and the MNE library. I was able to reproduce many of the findings of the original paper using the linear regression model. In addition to the effects of these variables on timing of ERPs that the original paper discusses, the linear regression's partial correlations and topographic maps that I plotted illuminate the relationship between each word attribute and the location of ERPs. For example, I found that visual complexity has an early negative effect in the frontopolar and frontal cortices, and a positive effect in the occipital area. But over time, that negative effect is more strongly concentrated in the central area and the positive effect diminishes. I found consonant vowel proportion to have an early negative effect on the central region as well. Orthographic disance has a strong positive effect in the frontal cortex around 300 ms. 
Each word attribute seems to have a concentrated effect in a particular brain region at certain times after stimulus presentation, though bigram frequency seemed to have the smallest effect. 

This analysis was performed mainly for my own education. Some key takeaways:
1. Learned the difference between epoch and evoked
2. Practiced with MNE Linear Regression function 
3. Learned how multiple regressions model EEG data
4. Practiced MNE topograph plotting
5. Drew conclusions on EEG correlates through Betas and T Values 
