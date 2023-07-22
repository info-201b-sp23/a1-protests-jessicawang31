# Assignment 1: Protests

During the past few years in the United States, there has been a surge of protests in support of the Black Lives Matter movement, women's rights, trans rights, immigration reform, gun control, the environment, and many other social and political issues.

In this assignment, you will work with data from [CountLove](https://countlove.org/), a group that collects data about protests from across the United States, including information about the purpose of the protests, the location of the protests, as well as how many people attended the protests. This data has often been [cited by the *New York Times*](https://www.nytimes.com/2020/08/28/us/black-lives-matter-protest.html), among other major outlets.

Through this assignment, you will be able to answer questions including:
- What were the most attended and least attended protests in the US in the last 5 years?
- How many protests occurred in Washington state?
- How did the number of protests in 2019 compare to 2020, and why?
- Why are people protesting in the US? What are the biggest motivators?


This assignment is divided into 2 parts. You will complete your coding work in the `analysis.R` file, and you will write short answer responses related to critical analysis and reflection of the data in this `README.md` file. Before getting started on your coding work, you should complete the section **"Critical Analysis & Reflection: Before You Code"** below.

When you are finished with the assignment, be sure to push all changes to your GitHub repository and then submit the link on Canvas.

## Before You Code: Critical Analysis & Reflection

Before diving into this (or any) dataset, it's important to know where the data came from, and it's important to have or to seek out _domain familiarity_ — in other words, knowledge about the subject/topic of the dataset. (We don't want to be "strangers in the dataset," as Catherine D'Ignazio and Lauren Klein describe it.)

To get more familiar, we are going to begin by doing some background reading.

- First, please read [this FAQ](https://countlove.org/faq.html) from the CountLove website and the opening of [this blog post](https://www.tommyleung.com/countLove/index.htm). Based on the information in these pieces, why did the creators start collecting the CountLove data? Please answer in 2-3 sentences (3 points)
  
  The creators of the CountLove data starting collecting data about aggregate protest data because they noticed there wasn't much readily available. The creators hope that this data become helpful for journalists and concerned citizens to understand these singular protests with the context of their trends as these protests represent a way of communication between citizens and elected officials.

- Next, we would like you to read this [*New York Times* piece, which uses CountLove data](https://www.nytimes.com/interactive/2020/06/13/us/george-floyd-protests-cities-photos.html) (here's a [Google Doc version for anyone who gets paywalled](https://docs.google.com/document/d/1sdjFsA5csYuH4plNEEk7WXT77K5h5ZuyW05CBwYdk6A/edit?usp=sharing)), and which describes the Black Lives Matter protests that occurred in the summer of 2020. Please summarize the main point or argument of this article in 2-3 sentences (3 points)
  
  This article brings awareness to the Black Lives Matter movement after the outrageous death of George Floyd. The map from this article shows data from all over American states where thousands of protests were being held, with people from all backgrounds, whether black, brown, white, or a mix, all demanding for racial justice and reform.

Next, we're going to reflect about who collected this data, and what's actually inside it.

- Who collected and shared the CountLove data, and what do they do for a living? Please answer in 1-2 sentences(2 points)

  The people who collected and shared the CountLove data are L. Nathan Perkins and Tommy Leung, who are both scientists and engineers. Nathan studies brains and how they can optically record and manipulate their neural activity for a living, whereas Tommy is an engineer and an amateur chef for fun.

- As Klein and D'Ignazio remind us, when it comes to data, "what gets counted counts." What types of demonstrations does CountLove include in their data, and what types do they exclude? (3 points)

  CountLove includes data that they count as public displays of protests that aren't part of "regular businesses." They do not include data from awareness or fundraising events, commemorative celebrations, historic reenactments, town halls, or campaign rallies. 

- How and where does CountLove get their data about the protests? Please answer in 2-3 sentences (2 points)

  CountLove gets their data about the protests from crawling local newspapers and television sites daily. These crawls is where most of their data comes from and crawling is the process of systematically browsing webpages, usually utilizing a software program to do so.

- How does CountLove make their estimates about the number of people who attended a protest? What potential problems might arise from this method of estimation? Please answer in 3-4 sentences (4 points)
  
  CountLove makes their estimates about the number of people who attend protests by recording the most conservative attendance number from the news articles they link and get their data from. They interpret "a dozen" as 10, "dozens" as 20, and "hundreds" as 100. Additionally, if the article doesn't provide a count, CountLove notes the protest but leaves the count empty. Potential problems that might arise from their method of estimation can lead to incorrect conclusions, especially problematic with larger datasets, which could   lead to a biased or skewed dataset and losing accuracy which could all lead to a misinterpretation from the audience using such data.
  
- What are two central values of Count Love? Name and briefly describe them. (See the Envisioning Cards for a defintion of "value".)

   Compassion and Connection are the two central values of CountLove. Compassion is being able to empathetic towards others and their situations and connection is being able to bond with others.

- Name and briefly describe one direct stakeholder and one indirect stakeholder (See the Envisioning Cards)?

  A direct stakeholder will be someone who uses the data provided in CountLove and an indirect stakeholder is someone who benefits from this data exiting, such as the protest attendees and the people who they are protesting for in some cases.

## While You Code: Critical Analysis & Reflection

- Reflection 1: Why do you think the mean is higher than the median? Which metric would you use in a report about this data, and why? Please answer in 2-3 sentences (2 points)

  The mean is higher than the median because the mean is affected by outliers whereas the median is not. Since the mean is greater than the median, it means the dataset is skewed right. We would wabt to use the median to report about this data because the mean is skewed due to the outliers in the dataset. 

- Reflection 2: Before actually calculating the number of protests that occurred in 2018, 2019, 2020, record your guesses for the following questions. (1 point)

  Guess: Do you think there were more protests in 2019 than in 2018? Why or why not? Please answer in 1 or 2 sentences
  
    I think there were more protests in 2018 because the COVID-19 pandemic started in late 2019 which
    could have restricted the amount of protests that could have occured in person.

  Guess: Do you think there were more protests in 2020 than in 2019? Why or why not? Please answer in 1 or 2 sentences
    
    I think there were more protests in 2020 than in 2019 becasue of the Black Lives Matter movement 
    that started bvecoming more widespread than before.

- Reflection 3: Does the change in the number of protests from 2018 to 2019 to 2020 surprise you? Why or why not? What do you think explains the fluctuation? Please answer in 1 or 2 sentences (2 points)

  I change in number of protests from 2018 to 2019 to 2020 does surprise me to an extend becasue the change 
from 2018 to 2019 does not surprise me as it declined and it was what I guessed as the pandemic started up.
However, the change from 2019 to 2020 did surprise me even though it was what I predicted, the increase 
was quite significant which is surprising becasue although BLM became more widespread, Covid was still 
very prominent.

- Reflection 4: What is the first and fourth most frequent category of protest? Do these frequencies align with your sense of the major protest movements in the U.S. in the last few years? Why or why not? (3 points)

  Racial injustice is the most frequent category of protest and civil rights is the fourth most frequent category of protests. I think these frequencies do align with my sense of the major protests in the U.S. in the last few years because most of the major protests have been ones related to things such as the Black Lives Movement which is a racial injustice protest and even civil rights. The civil rights category will alwasy be somewhat prevalent too as minorities, women, etc. will still always be looked down upon and considered lesser than by some people and these types of protests will continue to happen.
  
## After You Code: Critical Analysis & Reflection

In the second chapter of *Data Feminism*, Klein and D'Ignazio describe 4 ways that data scientists can challenge power and take action:
> Taking action can itself take many forms, and in this chapter we offer four starting points:  
> (1) Collect: Compiling counterdata—in the face of missing data or institutional neglect—offers a powerful starting point as we see in the example of the DGEI, or in María Salguero’s femicide maps discussed in chapter 1.  
> (2) Analyze: Challenging power often requires demonstrating inequitable outcomes across groups, and new computational methods are being developed to audit opaque algorithms and hold institutions accountable.  
> (3) Imagine: We cannot only focus on inequitable outcomes, because then we will never get to the root cause of injustice. In order to truly dismantle power, we have to imagine our end point not as “fairness,” but as co-liberation.  
> (4) Teach: The identities of data scientists matter, so how might we engage and empower newcomers to the field in order to shift the demographics and cultivate the next generation of data feminists?  

- How does the CountLove project embody one or more of these 4 forms of challenging power? Please answer in at least 3-4 sentences (3 points)

  The CountLove project embodies Collect and Analyze forms of challenging power. This is because CountLove collects their data from protests using various news sources and television programs. They do it to the best of their ability as not all information is there such as the number of attendees. They then upload this data for users to see and before doing so, they have to carefully analyze the data they've collected to ensure its accuracy.

- What is the most interesting or surprising thing you learned from this analysis? Please answer in at least 2-3 sentences (2 points)
  
  The most interesting thing I learned from this analysis is that RStudio is able to take in a crazy amount of data and not crash and is able to read and and extract specific columns from such a large dataset very quickly. It was interesting to see my code work and print out my variables and see the data that the console prints out.

- What is a kind of analysis that you would like to do or that would be interesting to do with the CountLove data that you don't have the time or skills to accomplish at this moment? Please answer in at least 2-3 sentences (2 points)

  I would be interested in seeing if there are subcategories in the large protest categories in the CountLove data. For example, racial injustice being the largest protest category, it would be interesting to analyze if there were subcategories such as racial injustice towards specific groups of individuals. 
