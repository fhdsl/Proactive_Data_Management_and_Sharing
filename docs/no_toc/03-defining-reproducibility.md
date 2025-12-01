# (PART\*) Effective Data Management {-}

# Defining reproducibility

In this section we will cover the following learning objectives:

<img src="03-defining-reproducibility_files/figure-html//10nOR2t1-F0E01fItN_l8uYRWslH2PmebPvhQzCBeCPM_g3896feb580f_16_18.png" alt="Learning Objectives: Understand the fundamental concepts of repeatability vs reproducibility vs replicability. Recognize how working to make your analyses reproducible saves you and your collaborators time. Explain how reproducibility is on a continuum. Describe how working toward reproducible analyses can assist in enhancing the accuracy of analysis results. " width="1250" style="display: block; margin: auto;" />

## What is reproducibility

There's been much discussion about what is included in the term `reproducibility` and there is some discrepancy between fields. For the broad field of cancer research, a _reproducible analysis is one that can be re-run by a different researcher, yet the same result and conclusion is found_.

<img src="03-defining-reproducibility_files/figure-html//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_146.png" alt="Reproducibility is a different analyst re­-performing the same analysis with the same code and data." width="1250" style="display: block; margin: auto;" />

Reproducibility is related to repeatability and replicability but it is worth taking time to differentiate these terms.

Perhaps you are like Ruby and have just found an interesting pattern through your data analysis! This has probably been the result of many months or years on your project and it's worth celebrating!

<img src="03-defining-reproducibility_files/figure-html//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_0.png" alt="Ruby the researcher has found something very interesting through data analysis. Ruby has a scatterplot on her computer that shows blue and pink data points and a trendline. The scatterplot has Variable A on the x axis and Variable B on the y axis. Ruby says my data analysis is showing a pattern that is very informative for ongoing research in my field." width="1250" style="display: block; margin: auto;" />

But before she considers these results a done deal, Ruby should test whether she is able to re-run her own analysis and get the same results again. This is known as _repeatability_.

<img src="03-defining-reproducibility_files/figure-html//10nOR2t1-F0E01fItN_l8uYRWslH2PmebPvhQzCBeCPM_g35294cebb05_0_482.png" alt="Repeatable means that if you keep everything the same but repeat the analysis (or experimental protocol) - do you get the same results? Ruby the researcher has her same code or experimental protocol and data but a repeat sign around them. If she re-runs the analysis, will she get the same scatterplot of results we’ve seen previously?" width="1250" style="display: block; margin: auto;" />

Given that Ruby's analysis is repeatable; she may feel confident now to share her preliminary results with her colleague, Avi the Associate. Whether or not someone else will be able to take Ruby's code and data, re-run the analysis, and obtain the same results is known as _reproducibility_. The same could be true for running the same experimental protocol with the same samples by another colleague.

<img src="03-defining-reproducibility_files/figure-html//10nOR2t1-F0E01fItN_l8uYRWslH2PmebPvhQzCBeCPM_g35294cebb05_0_146.png" alt="Reproducible: using the same data and analysis or experimental protocol but in the hands of another researcher - do we get the same results? Ruby the researcher sends her code and data to Avi the Associate who then tries to re-run the same analysis  on his own computer." width="1250" style="display: block; margin: auto;" />

If Ruby's results are able to be reproduced by Avi, now Avi may collect new data and use Ruby's same analysis methods to analyze his data (or collect new samples and run the same experimental protocol). Whether or not Avi's new data/samples and results concur with Ruby's study's original inferences is known as _replicability_.

<img src="03-defining-reproducibility_files/figure-html//10nOR2t1-F0E01fItN_l8uYRWslH2PmebPvhQzCBeCPM_g35294cebb05_0_644.png" alt="Replicable: with new data/samples do we obtain the same inferences? Ruby the researcher sends her code to Avi the Associate who then tries to re-run the same analysis on his own computer but now with new data (represented by a different color flashdrive). Will Avi come to the same inference that Ruby’s analysis did?" width="1250" style="display: block; margin: auto;" />

You may realize that these levels of research build on each other (like science is supposed to do). In this way, we can think of these in a hierarchy.  Skipping any of these levels of research applicability can lead to unreliable results and conclusions.

<img src="03-defining-reproducibility_files/figure-html//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1cd772e00_0_10.png" alt="A triangular graph shows a hierarchy of research. Repeatability is a the bottom ‘same researcher, same machine’, Runnability is next ‘same researcher, new machine’, Reproducibility is above that, ‘new researcher, same data’ and on the very top is Replicability ‘new researcher, new data’." width="1250" style="display: block; margin: auto;" />

Science progresses when data and hypotheses are put through these levels thoroughly and sequentially. If results are not repeatable, they won't be reproducible or replicable.

<img src="03-defining-reproducibility_files/figure-html//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_564.png" alt="If your results are not repeatable they will NOT be reproducible. In other words, if you can’t get the same answer twice, other researchers won’t be able to get your answer either." width="1250" style="display: block; margin: auto;" />

Ideally all analyses and results would be reproducible without too much time and effort spent; this would aid in the efficiency of research getting to the next stages and questions. But unfortunately, in practice, reproducibility is not as commonplace as we would hope. Institutions and reward systems generally do not prioritize or even measure reproducibility practices. Standards in research and training opportunities for reproducible techniques can be scarce. Reproducible research can often feel like an uphill battle that is made steeper by lack of training opportunities.

In this course, we hope to equip your research with the tools you need to enhance the reproducibility of your analyses so this uphill battle is _less steep_.

## Reproducibility in daily life

What does reproducibility mean in the daily life of a researcher?

Let's say Ruby's results are repeatable in her own hands and she excitedly tells her associate, Avi, about her preliminary findings. Avi is very excited about these results as well as Ruby's methods!

<img src="03-defining-reproducibility_files/figure-html//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_179.png" alt="Ruby the researcher has found something very interesting through data analysis. Ruby has a scatterplot on her computer that shows blue data points and an trendline that shows a positive correlation. The scatterplot has Variable A on the x axis and Variable B on the y axis. Avi the associate sees Ruby the researcher’s results and is also excited about the findings. Avi says Ruby’s findings are super relevant to my work and I’m interested in using her methods!" width="1250" style="display: block; margin: auto;" />

Avi is also interested in Ruby's analysis methods and results. So, Ruby sends Avi the code, data, and methods she used to obtain the results. Now, whether or not Avi is able to obtain the same exact results with this same data and same analysis code will indicate if Ruby's analysis is reproducible.

<img src="03-defining-reproducibility_files/figure-html//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_944.png" alt="Ruby the researcher has her computer with a plot and a significant and exciting research result. Ruby says 'Here, Avi, this code runs well on my computer, let me email it to you!' Avi the associate says 'so exciting'" width="1250" style="display: block; margin: auto;" />

Ruby may have spent a lot of time on her code and getting it to work on her computer, but whether it will successfully run on Avi's computer is another story. Often when researchers share their analysis code it leads to a substantial amount of effort on the part of the researcher who has received the code to get it working and this often cannot be done successfully without help from the original code author [@BeaulieuJones2017]. This same concept applies to experimental research methods in a laboratory setting.

Avi is encountering errors because Ruby's code was written with Ruby's computer and local setup in mind and she didn't know how to make it more generally applicable. Avi is spending a lot of time just trying to re-run Ruby's same analysis on her same data; he has yet to be able to try the code on any additional data (which will likely bring up even more errors). This is similar to trying to follow an experimental research method in the lab with vague or unclear instructions!

<img src="03-defining-reproducibility_files/figure-html//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_993.png" alt="Avi the associate is confused and sweating. His computer has the word ‘error’ written all over it and its on fire trying to use Ruby’s code on Ruby’s data. This is using a substantial amount of time and effort on Avi’s part. " width="1250" style="display: block; margin: auto;" />

Avi is still struggling to work with Ruby's code and is confused about the goals and approaches the code is taking. After struggling with Avi's code for an untold amount of time, Avi may decide it's time to email Ruby to get some clarity. Now both Avi and Ruby are confused about why this analysis isn't nicely re-running for Avi. Their attempts to communicate about the code through email haven't helped them clarify anything. Multiple versions of the code may have been sent back and forth between them and now things are taking a lot more time than either of them expected.

<img src="03-defining-reproducibility_files/figure-html//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_1066.png" alt="Ruby the researcher and Avi are emailing back and forth. Avi is very confused about Ruby’s code and data. Avi’s computer says 'Error: file path 'Ruby’s computer/Ruby’s file/final_version10.R' not found'. Avi email says ‘Re:Re:Re: Data Hi Ruby, I don’t understand what this code is supposed to be doing…’ Ruby is also confused and emails back to Avi 'Re:Re:Re: Data Hi Avi, It works for me?''" width="1250" style="display: block; margin: auto;" />

Perhaps at some point Avi is able to successfully run Ruby's code on Ruby's same data. Just because Avi didn't get any errors doesn't mean that the code ran exactly the same as it did for Ruby.

<img src="03-defining-reproducibility_files/figure-html//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1accd298e_0_673.png" alt="Ruby the researcher and Avi the associate are both very confused and slightly horrified that they both ran the same code and data but received different results." width="1250" style="display: block; margin: auto;" />

Lack of errors also doesn't mean that either Ruby or Avi's runs of the code ran with high accuracy or that the results can be trusted. Even a small difference in decimal point may indicate a more fundamental difference in how the analysis was performed and this could be due to differences in software versions, settings, or any number of items in their computing environments. This challenge also exists when trying to repeat a research method that you or someone else has written, especially if there aren’t enough details to precisely describe the conditions in which the data was collected.


## Reproducibility is worth the effort!

Perhaps you've found yourself in a situation like Ruby and Avi; struggling to re-run code or a method that you thought for sure was working a minute ago. In the upcoming chapters, we will discuss how to bolster your projects' reproducibility.

As you apply these reproducible techniques to your own projects, you may feel like it is taking more time to reach endpoints, but keep in mind that reproducible analyses and projects have higher upfront costs but these will absolutely pay off in the long run.

<img src="03-defining-reproducibility_files/figure-html//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf7bed24491_1_38.png" alt="Reproducibility is a tortoise’s game - it’s an incremental and slow process but it has high payoffs!" width="1250" style="display: block; margin: auto;" />

Reproducibility in your analyses is not only a time saver for yourself, but also your colleagues, your field, and your future self!

<img src="03-defining-reproducibility_files/figure-html//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1cd772e00_0_5.png" alt="Reproducible analyses save everyone time and effort!" width="1250" style="display: block; margin: auto;" />

You might not change a single character in your code or a step in your method but then return to it in a few days/months/years and find that it no longer runs! Reproducible code and research methods stands the test of time longer, making 'future you' glad you spent the time to work on it. It's said that your closest collaborator is you from 6 months ago but you don't reply to email [@Broman].

<img src="03-defining-reproducibility_files/figure-html//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1cd772e00_0_330.png" alt="Ruby the researcher’s code works now as represented on her computer by a check mark. But Future Ruby, who has gray hair has an error running the same code!" width="1250" style="display: block; margin: auto;" />

Many a researcher has referred to their frustration with their past selves:

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">Dear past-Hadley: PLEASE COMMENT YOUR CODE BETTER. Love present-Hadley</p>&mdash; Hadley Wickham (\@hadleywickham) <a href="https://twitter.com/hadleywickham/status/718203628528349184?ref_src=twsrc%5Etfw">April 7, 2016</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

The more you comment your code, or detail your method and make it clear and readable, your future self will thank you.

Reproducible code and research protocols also saves your colleagues time! The more reproducible your methods are, the less time your collaborators will need to spend troubleshooting it. The more people who use your methods need to try to troubleshoot it, the more time is wasted. This can add up to a lot of wasted time and effort.

<img src="03-defining-reproducibility_files/figure-html//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1cd772e00_0_160.png" alt="If Ruby’s code is less reproducible, every researcher who attempts to use Ruby’s code will encounter the same errors and each person will have to fix it. This adds up to a lot of spent researcher time and effort." width="1250" style="display: block; margin: auto;" />

But, reproducible code and methods saves everyone exponential amounts of time and effort! It will also motivate individuals to use and cite your methods in the future!

<img src="03-defining-reproducibility_files/figure-html//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf1cd772e00_0_53.png" alt="If Ruby’s code is built in a sturdier manner, it will save others’ time who might also need to perform a similar analysis. Ruby’s code is made reproducibly in this example and only one of her seven colleagues that are using her code needed to troubleshoot an error." width="1250" style="display: block; margin: auto;" />

## Reproducibility exists on a continuum!

Incremental work on your analyses is good! You do not need to make your analyses perfect on the first try or even within a particular time frame. The first step in creating an analysis is to get it to work once! But the work does not end there. Furthermore, no analysis is or will ever be perfect in that it will not be reproducible in every single context throughout time. Incrementally pushing our analyses toward the perfect side of the continuum is the goal.

<img src="03-defining-reproducibility_files/figure-html//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf7bed24491_1_0.png" alt="Reproducibility is on a continuum. This graph shows a two sided arrow with a gradient. On the very left is a ‘not repeatable analysis’ it was ran once. To the right of that is an analysis that ‘re-runs sometimes’. To the right of this, is an analysis that ‘Re-runs reliably in most contexts’.  And all the way to the right is a ‘perfectly reproducible analysis’ that ‘Re-runs in every situation and gets the same result every time’. In red lettering we note that every analysis is started by being run once but no analysis is ‘perfectly reproducible’." width="1250" style="display: block; margin: auto;" />


## Reproducibility practices helps rigor

If your analysis is not transparent it is difficult for others to discern how correct it is. Also, if you can't get the same results twice, you shouldn't trust your analysis yet, as something might be missing from your code or protocol. Therefore, reproducibility practices can help ensure that our work is as correct as our current understanding of methods. 

If our understanding of methods changes, for example we learn that we need to use a new normalization technique to mitigate for batch effects, we can still find value in our older research if it is clear exactly how the work was done. We can use our previous data and update or methods using new techniques much more easily.


In Summary, while it takes extra effort upfront to make your research follow best practices for reproducibility, it ultimately saves you much more time in the end and makes your work much more transparent to others and you future self. Remember that being reproducible means that your work can be consistently redone with the same results, **it does not necessarily mean that it is correct**. However, this consistency is the first step to ensure that your science is rigorous and enables you and others to more deeply understand why others may or may not reproduce your work in the future. 
