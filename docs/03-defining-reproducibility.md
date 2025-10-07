# (PART\*) Effective Data Management {-}

# Defining reproducibility

In this section we will cover the following learning objectives:

![](03-defining-reproducibility_files/figure-docx//10nOR2t1-F0E01fItN_l8uYRWslH2PmebPvhQzCBeCPM_g3896feb580f_16_18.png)

## What is reproducibility

There's been much discussion about what is included in the term `reproducibility` and there is some discrepancy between fields. For the broad field of cancer research, a _reproducible analysis is one that can be re-run by a different researcher and the same result and conclusion is found_.

![](03-defining-reproducibility_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_146.png)

Reproducibility is related to repeatability and replicability but it is worth taking time to differentiate these terms

Perhaps you are like Ruby and have just found an interesting pattern through your data analysis! This has probably been the result of many months or years on your project and it's worth celebrating!

![](03-defining-reproducibility_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_0.png)

But before she considers these results a done deal, Ruby should test whether she is able to re-run her own analysis and get the same results again. This is known as _repeatability_.

![](03-defining-reproducibility_files/figure-docx//10nOR2t1-F0E01fItN_l8uYRWslH2PmebPvhQzCBeCPM_g35294cebb05_0_482.png)

Given that Ruby's analysis is repeatable; she may feel confident now to share her preliminary results with her colleague, Avi the Associate. Whether or not someone else will be able to take Ruby's code and data, re-run the analysis and obtain the same results is known as _reproducibility_. The same could be true for running the same experimental protocol with the same samples by another colleague.

![](03-defining-reproducibility_files/figure-docx//10nOR2t1-F0E01fItN_l8uYRWslH2PmebPvhQzCBeCPM_g35294cebb05_0_146.png)

If Ruby's results are able to be reproduced by Avi, now Avi may collect new data and use Ruby's same analysis methods to analyze his data (or collect new samples and run the same experimental protocol). Whether or not Avi's new data/samples and results concur with Ruby's study's original inferences is known as _replicability_.

![](03-defining-reproducibility_files/figure-docx//10nOR2t1-F0E01fItN_l8uYRWslH2PmebPvhQzCBeCPM_g35294cebb05_0_644.png)

You may realize that these levels of research build on each other (like science is supposed to do). In this way, we can think of these in a hierarchy.  Skipping any of these levels of research applicability can lead to unreliable results and conclusions.

![](03-defining-reproducibility_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1cd772e00_0_10.png)

Science progresses when data and hypotheses are put through these levels thoroughly and sequentially. If results are not repeatable, they won't be reproducible or replicable.

![](03-defining-reproducibility_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_564.png)

Ideally all analyses and results would be reproducible without too much time and effort spent; this would aid in the efficiency of research getting to the next stages and questions. But unfortunately, in practice, reproducibility is not as commonplace as we would hope. Institutions and reward systems generally do not prioritize or even measure reproducibility practices. Standards in research and training opportunities for reproducible techniques can be scarce. Reproducible research can often feel like an uphill battle that is made steeper by lack of training opportunities.

In this course, we hope to equip your research with the tools you need to enhance the reproducibility of your analyses so this uphill battle is _less steep_.

## Reproducibility in daily life

What does reproducibility mean in the daily life of a researcher?

Let's say Ruby's results are repeatable in her own hands and she excitedly tells her associate, Avi, about her preliminary findings. Avi is very excited about these results as well as Ruby's methods!

![](03-defining-reproducibility_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_179.png)

Avi is also interested in Ruby's analysis methods and results. So, Ruby sends Avi the code, data, and methods she used to obtain the results. Now, whether or not Avi is able to obtain the same exact results with this same data and same analysis code will indicate if Ruby's analysis is reproducible.

![](03-defining-reproducibility_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_944.png)

Ruby may have spent a lot of time on her code and getting it to work on her computer, but whether it will successfully run on Avi's computer is another story. Often when researchers share their analysis code it leads to a substantial amount of effort on the part of the researcher who has received the code to get it working and this often cannot be done successfully without help from the original code author [@BeaulieuJones2017]. This same concept applies to experimental research methods in a laboratory setting.

Avi is encountering errors because Ruby's code was written with Ruby's computer and local setup in mind and she didn't know how to make it more generally applicable. Avi is spending a lot of time just trying to re-run Ruby's same analysis on her same data; he has yet to be able to try the code on any additional data (which will likely bring up even more errors). Imagine a trying to follow an experimental research method in the lab with vague or unclear instructions!

![](03-defining-reproducibility_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_993.png)

Avi is still struggling to work with Ruby's code and is confused about the goals and approaches the code is taking. After struggling with Avi's code for an untold amount of time, Avi may decide it's time to email Ruby to get some clarity. Now both Avi and Ruby are confused about why this analysis isn't nicely re-running for Avi. Their attempts to communicate about the code through email haven't helped them clarify anything. Multiple versions of the code may have been sent back and forth between them and now things are taking a lot more time than either of them expected.

![](03-defining-reproducibility_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_1066.png)

Perhaps at some point Avi is able to successfully run Ruby's code on Ruby's same data. Just because Avi didn't get any errors doesn't mean that the code ran exactly the same as it did for Ruby.

![](03-defining-reproducibility_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_673.png)

Lack of errors also doesn't mean that either Ruby or Avi's runs of the code ran with high accuracy or that the results can be trusted. Even a small difference in decimal point may indicate a more fundamental difference in how the analysis was performed and this could be due to differences in software versions, settings, or any number of items in their computing environments. This challenge also exists when trying to repeat a research method that you or someone else has written, especially if there aren’t enough details to precisely describe the conditions in which the data was collected.


## Reproducibility is worth the effort!

Perhaps you've found yourself in a situation like Ruby and Avi; struggling to re-run code or a method that you thought for sure was working a minute ago. In the upcoming chapters, we will discuss how to bolster your projects' reproducibility.

As you apply these reproducible techniques to your own projects, you may feel like it is taking more time to reach endpoints, but keep in mind that reproducible analyses and projects have higher upfront costs but these will absolutely pay off in the long term.

![](03-defining-reproducibility_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf7bed24491_1_38.png)

Reproducibility in your analyses is not only a time saver for yourself, but also your colleagues, your field, and your future self!

![](03-defining-reproducibility_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1cd772e00_0_5.png)

You might not change a single character in your code or a step in your method but then return to it in a few days/months/years and find that it no longer runs! Reproducible code and research methods stands the test of time longer, making 'future you' glad you spent the time to work on it. It's said that your closest collaborator is you from 6 months ago but you don't reply to email [@Broman].

![](03-defining-reproducibility_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1cd772e00_0_330.png)

Many a researcher has referred to their frustration with their past selves:

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">Dear past-Hadley: PLEASE COMMENT YOUR CODE BETTER. Love present-Hadley</p>&mdash; Hadley Wickham (\@hadleywickham) <a href="https://twitter.com/hadleywickham/status/718203628528349184?ref_src=twsrc%5Etfw">April 7, 2016</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

The more you comment your code, or detail your method and make it clear and readable, your future self will thank you.

Reproducible code and research protocols also saves your colleagues time! The more reproducible your methods are, the less time your collaborators will need to spend troubleshooting it. The more people who use your methods need to try to troubleshoot it, the more time is wasted. This can add up to a lot of wasted time and effort.

![](03-defining-reproducibility_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1cd772e00_0_160.png)

But, reproducible code and methods saves everyone exponential amounts of time and effort! It will also motivate individuals to use and cite your methods in the future!

![](03-defining-reproducibility_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1cd772e00_0_53.png)

## Reproducibility exists on a continuum!

Incremental work on your analyses is good! You do not need to make your analyses perfect on the first try or even within a particular time frame. The first step in creating an analysis is to get it to work once! But the work does not end there. Furthermore, no analysis is or will ever be perfect in that it will not be reproducible in every single context throughout time. Incrementally pushing our analyses toward the right of this continuum is the goal.

![](03-defining-reproducibility_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf7bed24491_1_0.png)

In Summary, reproducibility is on a continuum. You can improve your practices over time. While it takes extra effort upfront to make your research follow best practices, it saves. you much more time in the end and makes your work much more transparent to others and you future self. Remember that being reproducible means that your work can be consistently redone to get the same result, it does not necessarily mean that it is correct. However, this consistency is the first step to ensure that your science is rigorous and enables you and others to more deeply understand why others may or may not reproduce your work in the future. 
