---
layout: post
title: How to Transition from Academia to Data Science
date: 2017-12-24
comments: true
---



![](https://media-exp2.licdn.com/mpr/mpr/AAEAAQAAAAAAAAyEAAAAJDg1ZTIwZTk0LThiZDgtNDczOC1hMDMwLTRmMzc2YjA3NjdkNw.jpg)

It has now been about 4 months since I quit my job as a tenure track professor at an R1 university to take a position as a data scientist in Silicon Valley.  I would be lying if I said the transition has been 100% smooth.  But even so, I am still deliriously happy that I managed to get out!  Despite the complete shock of many of my colleagues that I gave up the "dream job for life" (see some of my previous posts), I have also had several colleagues, primarily some of the my more junior friends, tell me that they are contemplating the same move but do not know how to start.  So I figured that was worth at least a blog post or two.

First things first...my experiences are just my experiences.  YMMV on anything I post here.  Second, I can only write this from my perspective, which is that of someone with a PhD in nuclear engineering from the number 1 ranked graduate school in the field.  After getting my PhD, I went to work in the national lab system for a while and then in the federal government in reearch positions.  I returned to academia after spending 10 years outside it and then spent 5 years on the tenure track.  So my thoughts on this subject are for people who have spent some time in full-out academia and do not necessarily apply to people moving from graduate school or a postdoc position to data science.  The difference here is that coming out of those positions your career is essentially still a blank canvas whereas those who have spent time working as academics are going to have been programmed into certain ways of thinking and doing things.  Those of you straight out of school or postdoc should have a _much_ easier time with both finding a job as well as making the transition to the culture than those who have worked in academia for a little while.

So with that caveat out of the way, here is a random assortment of observations and suggestions should you decide to make the move.


**1. Accept (and embrace the fact) that you are an expert in a very narrow field**

This is, in fact, the whole point of getting a PhD and then working in academia -- to develop a research expertise that nobody in the world has.  Upon my return to academia, I quickly landed some funding to bridge the gap between nuclear engineering (radiation detection for nuclear emergency response, to be precise) and so-called "big data" (a term that pretty much nobody uses anymore).  I am certainly an expert in the former, but knew nothing about the latter.  Recognizing this was key.  I knew that I knew nothing but needed to learn very quickly.  As a result, I attended an 8-week intensive program through [The Data Incubator](https://www.thedataincubator.com/) whose purpose is to turn people with PhDs in STEM disciplines into data scientists.  While attending the course was a tremendous sacrifice and burden on my family, it is really what enabled me to be ready to apply for jobs in data science.

This is for two reasons.  First, I certainly knew how to program, but not in languages relevant to data science (see below).  Second, (and I cannot emphasize this one enough), _professors are not taught to program like data scientists._ What I mean by this is that we frequently assign programming tasks to our graduate students, but we are not the ones who are sitting there trying to debug code or milk every last drop of efficiecy out of code.  Yet this will absolutely be expected of you as a data scientist.  You need to be prepared for this.

Data scientists need to be generalists.  Depending on the job you land this might be more or less true.  For instance, if you are working in a large company, you might have the opportunity to focus strictly on machine learning (ML) and leave the other tasks to other employees.  However, in small companies, the data scientist might be expected to also be the person standing up cloud clusters for running calculations, maintaining databases, or even advising on general IT infrastructure.  Know what you are and are not willing to do and seek out the companies

**2. Get the relevant skills**

Repeat after me: _no self-respecting data scientist uses Excel_ (other than to balance your checkbook).  For academics, I will also add that _no self-respecting data scientist uses Matlab._ 

I know I was kind of aghast to learn of that last one.  I mean, we PUBLISH with Matlab!  What the hell?!?  Yes, I know they have some nice ML tools and what not.  But first off, you cannot create productionalized code with it, regardless of what the sales people tell you.  Second, Matlab actually costs a lot of money outside of universities.  And yet Python is free, has great data science libraries, and can be productionalized.

So with those statement out of the way, here is a list of programming tools that a professor will need to learn.  You will not need to learn all of them, but what you do learn needs to be at a _very_ sophisticated level.  In general, you want at least one solid programming language along with all relevant packages, some form of SQL, and definitely the ability to work with the command line on either Mac or Linux.  (Oh yeah...I forgot to mention that _most data scientists avoid Windows like the plague._) 

- Python (by far the most common language among data scientists), including the following packages:
    - pandas
    - numpy
    - scipy
    - scikit-learn
    - matplotlib and/or seaborn
- R (not as common as Python, but still solid), but I don't know the packages since I don't use it
- SQL
    - most SQL variants behave the same
    - still, it is good to understand some of subtle variations
- Spark
    - PySpark
    - Scala Spark
    - SparkR
    - Hadoop is dead.  Long live Hadoop.
- Bash
    - You must be able to use the command line.  This is not negotiable.

**WARNING: CONTROVERSIAL STATEMENT AHEAD**

In addition to not all programming languages being equal, not all courses in programming are created equal.  When I was a professor, I was working at a university that housed one of the top 5 computer science departments in the country.  And I can tell you that what is being taught there on data science does _NOT_ meet the demands of serious companies in Silicon Valley.  The reason is that most of the professors there have been locked in the ivory tower for decades and have never actually WORKED in industry before, so they do not understand what matters to them.  For example, when students are taught SQL, they are taught the concept of an inner, and it is just second nature to them that this is how you bring together two tables.  Yet if you are just happily going about doing a zillion inner joins on a large dataset, you will find that to be a quick road to unemployment.  The reason is the inner join, the common, go-to tool that we learn in any SQL class, is very slow and memory intensive.  There are other ways of programming that will be much more efficient (see Common Table Expressions) that you can and should use.

True story: if you seek proof that academia has no idea how to teach data science, let me tell you about a real conversation I had with professors on a data science committee on campus.  

_Prof. A: We should go to some companies and get them to give us their data to teach with and analyze with our great tools._

_Prof. B: Yeah, but if they won't do that, I know that there is a lot of data out there on soccer.  Maybe we could analyze that._

Here are the problems with both of these statements.  Prof. A wants data from companies.  Great.  However, data is a form of currency to companies.  They will not just part with their data for free.  This statement demonstrates the naivety and disconnect between academia an industry.  Prof. B, on the other hand, is clearly unaware of what has already been done in data science, and done famously.  Have you never seen [Moneyball](http://www.imdb.com/title/tt1210166/?ref_=nv_sr_1)?  Ever heard of [Nate Silver](https://en.wikipedia.org/wiki/Nate_Silver) and his blog, [fivethirtyeight](http://fivethirtyeight.com/)?  Yes, ladies and gentlemen, this out of the mouths of people that are paid hundreds of grand a year and to whom students pay tens of thousands in tuition to.  


**3. Converting your CV to a resume**

This is where the rubber meets the road.  How will you really get the attention of data science hiring managers and recruiters?  After all, unless you have a PhD in computer science or statistics, you will not look like a "normal" applicant.

This part is going to be hard for most academics.  We have spent a career building up the glorious CV full of publications, invited talks, teaching assignments, and committee work.  I am going to warn you, this statement will hurt: **nobody gives a shit about your CV.**  There.  I said it.  

In order to apply for a data science jobs, you need to create a 1 page resume.  I am telling you right now that you cannot argue with me on the page limit.  No, you cannot spill over onto two pages.  You really must boil down your life into 1 page.  This resume needs to have the following sections IN THIS ORDER:

- Name and contact information
    - include a link to your GitHub profile (yes, you should have one...see below)
- Summary of qualifications
    - 1-2 sentences on how you are a data scientist
    - do NOT focus on your expertise in your academic field
- Experience
    - Position title
    - Employer
    - Dates of employment
    - VERY brief discription of the role (1-2 sentences max)
- Degrees obtained
    - one line per degree
    - do NOT include titles of dissertations, your advisor's information, etc.
- Additional training
    - Data science intensives
    - MOOC certifications
    - keep this data science specific
- Computer skills
    - a laundry list of the programming languages you a proficient in, cloud platforms you use, etc.


Yes, this downplays your education and plays up experience.  Because that is what matters to these people.  

And because experience is what matters, you need to be able to demonstrate that experience.  This is where your [GitHub](http://www.github.com) profile comes in.  You need to have samples of your data science work here.  These should ideally be in the form of Jupyter notebooks complete with plots and a LOT of descriptions and comments.  If you do not have actual work products you can show (meaning you have done analysis on some company data somewhere), you should go work on a [Kaggle](http://www.kaggle.com) problem or two.  This is not as good has having real-world experience since you are provided with the data you need to solve the problem and don't actually have to go out and find that data yourself.  But it is still better than nothing.  And then Kaggle data is preferrable to data from courses you might have taken where you were still learning a thing.

I am not kidding though when I say that most of your CV will be left on the cutting room floor.  Yes, I am sure your publications were glorious and that grant you landed was obviously hugely impactful.  **NOBODY IN THIS WORLD CARES.** If that is a reality that you cannot accept, then you might not be well suited to working in data science.  Sorry.


**4. You will be expected to show your chops at a technical interview**

Some companies in Silicon Valley are legendary for their white boarding sessions.  In these interviews, you will be given a very short period of time (think 2-5 minutes) to code something on the board or to solve a statistics problem while everyone is watching.  You will not be allowed access to reference material.  I found this process worse than my qualifying exams.  

You cannot successfully make it past this stage without practice!  There are many [awesome resources](https://github.com/yangshun/tech-interview-handbook) online.  I suggest you practice them, and do them in a timed 
