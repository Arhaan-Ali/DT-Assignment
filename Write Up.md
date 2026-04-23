# Write Up

The assignment started with me reading about all the 3 axis from the given sources and then I moved forward to the book **Designing Quality Survey Questions** by  **Leonard Bickman** and **Debra J. Rog** to understand what i am doing, then i started reading other surveys which the book suggested. I couldn't find any particular tests or surveys for the other 2 axis, so it was mostly based on what I thought about how the questions should be for those two axis. 

# Decision Tree making process
I started with heavy inspiration from the example JSON file given in the Github link.

***Question 1***
*"Choose the option that best matches how today felt."*

- This question makes a good start that's why i copied it from the example json file was given 
- To make it more natural for the users who were gonna use i added a 3rd type of ***collaborative*** options in further questions, which were internally adding values in internal or external for example *(0.25 internal + 0.75 external)*.

***Question 2***
*The question was depended to what the person has replied to it*

- This was done to make the decision more modular to various behaviors 

***Question 3***
*Looking back, How much of today’s outcome do you think was shaped by your actions?* 

Third question was making in thought that even if the user tries to gamify this process to answer only right questions according to them, it still gives a them a chance to think about what they had done throughout the day, might help them to think about the consequences of their actions the next days.

***Question 4***
*Think about one difficult interaction you had today. how could it have been better?*

This question was with the though that maybe the employee might have an interaction with someone that they didn't liked or made them regret whatever might be the case this question helps us answer our questions while keeping the user busy thinking about the interaction.

***Question 4***
*Think about today, did you find yourself giving more or receiving more?*
Only questions which i think could give away what might be the goal of this survey/questionnaire but equally important for our end goal

***Question 5***
*In a team setting, what feels more natural to you?*

In the book it  was advised to keep the hypothetical questions to minimum so i have kept it just one, where it would help the most to understand the thought process of the employee while making them reflect on their decisions they might have been making or make in the future.

The rest of the questions were also with similar though processes and i kept making them better by getting various versions of them through different ai models i tried some of their prompts but also tried to keep the answers reflections and the bridges humane so that it doesn't feel robotic.

## Changes made after creating personas

After creating the first draft of the JSON file that the chatbot was supposed to use, i ran it on various personas the first one was the hardest one to make right it was of a gen z employee who has lots of knowledge about mental health parameters and he worked in pattern recognition and AI/ML related topis 

###  Persona 1
*Name: Aarav Mehta*  
*Age: 23*  
*Role: AI/ML Engineer*

*Background:*
*Graduated early with a Computer Science degree. Built multiple side projects in mental health tech (journaling apps, mood trackers, behavioral analytics tools). Deeply interested in how cognition, emotion, and decision-making interact with technology. Self-taught in psychology alongside engineering.*
 
### Changes made according to Persona 1 
The goal was to not make the day reflection activity a game for him and also to keep the spirit of what we want to achieve. 

- When i ran the persona simulation on both gpt and claude both advised to remove options which were showcasing explicitly which options were right and which were wrong or unwanted, so I tried to remove them.
-  Gpt advised to add more blended options but according to me having collaborative answers was enough otherwise the end goal of the reflection activity were going to deteriorate.
- The main idea was to disguise to options better for someone who can understand patterns 
- Gpt and claude also advised to remove bridges but instead of removing them i made them more neutral.
- Gpt and claude also advised to make the flow of question randomized but i was aske to keep a concrete flow of these questions so i avoided that

### Persona 2 
Name: Rajiv Malhotra  
Age: 62  
Role: Senior Operations Director

Background:  
Started his career in the late 80s when systems were manual, hierarchies were rigid, and results mattered more than processes. Rose through the ranks purely on consistency, discipline, and sharp decision-making. Built teams from scratch, handled crises without frameworks, and learned everything on the job—no formal “leadership programs,” just experience.

- The second persona was made on the type of people on which these questions would work without a fail, and they would most probably answer honestly so there wasn't much to change here. 

### Persona 3 
Name: Karan Khanna  
Age: 33  
Role: Product Manager / Engineering Lead

Background:  
Started as a developer during the early boom of startups and rapidly evolving tech stacks. Put in long hours in his 20s—shipping features, switching companies smartly, and building a strong financial base. Transitioned into a managerial role after proving both technical and decision-making ability. Has seen tech evolve from relatively stable stacks to today’s fast, AI-driven chaos.

- Both gpt and claude concluded that this persona will not be able to completely gamify this questionnaire even on a day where he wants to look good, so in conclusion the flow questions was a little success. 

## Chat Bot Making Process
I asked **Claude** to make the chatbot and i told it to give a single html file with the UI being in *dark mode* and in **matte colors** with the UI showcasing it welcoming and professional.

The code is run in html runs without any local hosts and any npm needs best for showcasing the example of the flow of the decision tree

