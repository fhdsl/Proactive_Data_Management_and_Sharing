


# Creating clear documentation

Our goal for documentation is to be as comprehensive, navigable, and as always, as _clear_ as possible.

## Characteristics of clear documentation

### Is easy to find

No matter how well your documentation is crafted, it is of no use if no one can find them. Having documents that are standard and at the top of your directory is key. READMEs for example are standard documents in software that give the TL;DR of the project. In science, READMEs are incredibly valuable.

### Is comprehensive

All items are covered in the documentation in an organized fashion -- every. single. thing.
This includes all:

- Data sources and versions
- Metadata
- Software dependencies and their versions
- Terms
- Functions
- Arguments
- Parameters
- Defaults

**The most useful documentation...**  

- Not only define the items and files included, but tells how it relates to other items (and they have links where relevant).
- Make any existing defaults and calculations very clear. It doesn't assume that just because a term is used, the calculation is obvious. For example, Tumor Mutation Burden is a common statistic to report but it is calculated different ways. Documentation should describe major calculations and not assume standardization.
- Shows how to re-run the entire analysis, example lines of code go a long way.
- Tries to avoid the use of jargon, but if it is absolutely necessary to use a jargon-y term it links to information about the meaning of the term.

### Data formats are described

Perhaps after installation, getting data formatted correctly is one of the other very large hurdles users will need to deal with.

Ideally, your software can use a data format that is common. But the more that your tool is particular about an odd data format, the more your documentation needs to be specific about what the odd data format looks like. It's very helpful to include subsetted, de-identified example files for a positive control/example.

## Types of documentation you should have

Documentation strategies are not one size fits all but there are two types of documentation we strongly advise every project has: READMEs and analysis notebooks.

We refer you to see the [OpenPBTA project](https://github.com/AlexsLemonade/OpenPBTA-analysis) as a real life example of well documented open source data analysis.

### READMEs!

READMEs are also a great way to help your collaborators get quickly acquainted with the project.

![](11-creating-guides_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf8379bb805_0_11.png)

READMEs stick out in a project and are generally universal signal for new people to the project to start by READing them. GitHub automatically will preview your file called "README.md" when someone comes to the main page of your repository which further encourages people looking at your project to read the information in your README.

**Information that should be included in a README:**

1) General purpose of the project
2) Instructions on how to re-run the project
3) Lists of any software required by the project
4) Input and output file descriptions.
5) Descriptions of any additional tools included in the project?

You can take a look at this [template README](https://raw.githubusercontent.com/jhudsl/Reproducibility_in_Cancer_Informatics/main/resources/README-template.md) to get your started.

#### More about writing READMEs:

- [How to write a good README file](https://www.freecodecamp.org/news/how-to-write-a-good-readme-file/)
- [How to write an awesome README](https://towardsdatascience.com/how-to-write-an-awesome-readme-68bf4be91f8b)

### Exercise: Write a README for your project!

1. Download this [template README](https://raw.githubusercontent.com/jhudsl/Reproducibility_in_Cancer_Informatics/main/resources/README-template.md).
2. Fill in the questions inside the `{ }` to create a README for this project.
3. You can reference the "final" versions of the README, but keep in mind it will reference items that we will discuss in the "advanced" portion of this course. See the [R README here](https://github.com/jhudsl/reproducible-R-example) and the [Python README here](https://github.com/jhudsl/reproducible-python-example).
4. Add your README and updated notebook to your GitHub repository. Follow [these instructions to add the latest version of your notebook to your GitHub repository](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository#adding-a-file-to-a-repository-on-github). Later, we will practice and discuss how to more fully utilize the features of GitHub but for now, just drag and drop it as the instructions linked describe.

### Notebook descriptions

The generous use and keeping of notebooks is a useful tool for documentation of the development of an analysis.

Data analyses can lead one on a winding trail of decisions and side investigations, but notebooks allow you to narrate your thought process as you travel along these analyses explorations!

![](11-creating-guides_files/figure-docx//1LMurysUhCjZb7DVF6KS9QmJ5NBjwWVjRn40MS9f2noE_gf8f405fdab_0_186.png)

**Your scientific notebook should include descriptions that describe:**   

#### The purposes of the notebook

What scientific question are you trying to answer? Describe the dataset you are using to try to answer this and why does it help answer this question?

#### The rationales behind your decisions

Describe why a particular code chunk is doing a particular thing -- the more odd the code looks, the greater need for you to describe why you are doing it.

Describe any particular filters or cutoffs you are using and how did you decide on those?

For data wrangling steps, why are you wrangling the data in such a way -- is this because a certain package you are using requires it?

#### Your observations of the results

What do you think about the results? The plots and tables you show in the notebook -- how do they inform your original questions?

## How to keep your documentation up to date

![](11-creating-guides_files/figure-docx//1PH9_KlLVggYpNJI0fgvcIcft2vDtGA_mlCqKFA8gnAg_gd5f2c75a67_0_0.png)

### The goal of documentation maintenance

Perhaps you’ve been making improvements or otherwise updating your software tool. That's excellent and you deserve a big kudos for continuing maintenance on your tool!

But your work is not done yet. For each (user-facing) update you make to the tool, you should also make a documentation update. As a user, the only thing worse than having a tool with no documentation at all is having a tool with documentation that is out of date or otherwise incorrect.

![](11-creating-guides_files/figure-docx//1PH9_KlLVggYpNJI0fgvcIcft2vDtGA_mlCqKFA8gnAg_gd5f2c75a67_0_5.png)

If documentation updates aren't prioritized, your tool can easily get several versions ahead leaving the documentation you carefully crafted rather useless and misleading.

### Keep your documentation in one, version-controlled place

Presumably you have some sort of process for version controlling your tool updates (we assume GitHub but could be other services). Ideally, your documentation should be version controlled similarly and, if appropriate, in the same place.
The easier you make it on yourself to update your documentation, the more likely future you will be at updating it successfully! It's worth spending time thinking about your own development process and how you can make it easier on yourself and your team for longer-term better maintained documentation.

### Do not consider a tool fix done before its relevant documentation update is also completed

However you track your tasks, also track your documentation issues and always pair a software fix with a documentation fix -- or at least check if it affects anything user-facing. To help you remind you of this, you may want to use an [issue template](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository) (if you use GitHub) and make sure that issue template includes a reminder to update documentation.

### Make sure links work

A very simple but all too common problem with out of date documentation is broken links!

![](11-creating-guides_files/figure-docx//1PH9_KlLVggYpNJI0fgvcIcft2vDtGA_mlCqKFA8gnAg_gd5f2c75a67_0_37.png)

You can catch these broken links by manually clicking on all your links, but sometimes broken links will still slip through the cracks anyway! There are GitHub actions and other automated tools that can check your URLs for you. Take advantage of automation to do this for you so you can save your time an effort for other improvements to your tool and documentation!

Here's some options for automated URL-checking:  

- [GitHub action: urlchecker-action](https://github.com/marketplace/actions/urlchecker-action).  
- [GitHub action: URL checker](https://github.com/marketplace/actions/url-checker).  
- [6 Tools to Find Broken Links on Your Website](https://www.outlookstudios.com/tools-to-find-broken-links-on-your-website/) [@OutlookStudios2020].  

### Set aside time to do maintenance

In an academic setting it can be hard to find time for things that don't have urgent deadlines. But long term we know maintenance is best done little by little. In order to best maintain your work long term its best to set aside time on your calendar to actually do the maintenance. Otherwise it may never happen.

We encourage funding institutions to recognize that maintenance is the most frugal strategy. Whether it be for software or course or other products, maintenance should be prioritized for the long term benefit of the research community. More funding opportunities should be set aside for maintenance of current products as opposed to always creating new products that will also decay if not maintained.

## Exercise 1: Add a reminder for documentation updates to your task manager

- If you use GitHub, add an [issue template](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository) that has a reminder to update documentation.  
- If you use something else for task management, look for some other way to remind yourself (and your fellow developers on the project) to keep documentation up-to-date for each change.


## Exercise 2: Implement a URL checker

- If you use GitHub for your documentation, add a url checking GitHub action to your repository.
We used a url-checker GitHub action for developing this course!
You can see [ours here for an example](https://github.com/jhudsl/ottr-reports).  
- If you use something else for version control, look into URL checkers that you can easily implement into your development process.  
