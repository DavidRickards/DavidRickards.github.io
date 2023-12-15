---
layout: essay
type: essay
title: "AI : Balance bewteen Friend & Foe In The Classroom"
# All dates must be YYYY-MM-DD format!
date: 2023-11-20
published: true
labels:
  - Software Engineering
  - Learning
  - AI
  - ChatGPT
---

#  Introduction
The integration of Artificial Intelligence (AI) in school education is starting to change the learning environment, presenting new possibilities and tools for students to improve their learning experience. The role of AI has growing relevance to the field of software engineering as it provides a way for students to learn and be exposed to advanced tools and techniques to tackle complex coding solutions. The only AI that I have used in software engineering is every students best friend, [ChatGPT](https://chat.openai.com/), to help assist me in breaking down complex or confusing tasks to better my own skills, reduce the amount of time it takes to write certain code,  and teach me how to code things that I would not normally know.
<img src="https://www.brookings.edu/wp-content/uploads/2023/01/shutterstock_2237655785.jpg?w=1500" width="300px">


# Me, Myself, & AI Experiences in 314
## Experience / In-class / Practice WODS
In my software engineering class, I had to complete  a "WOD," which were these in-class assignments that had to be functional and finished within the limited time to pass. Sometimes, practice WODs were assigned as homework, and we could make multiple attempts to solve them. For all of the practice WODs, if there was not a video that I watched and followed along with at some point, then I ended up using ChatGPT to help me solve them. ChatGPT was a lifesaver because of how quickly it could produce code with prompts related to or taken from the in-class WOD. I am not the fastest typer, and I didn’t have knowledge of many of the code's methods, so I would often use ChatGPT to generate this code much faster than I could to save precious time.

One time, when we were working on the surfing prompt in one of our earliest WODs, I was completely stuck, and I was getting a different output than I was supposed to get. So, I copied the whole prompt over to ChatGPT and retried the code, and it gave the correct output. I passed the WOD, but I never really figured out what the issue was and thus was never able to learn from that mistake. I tried to avoid doing that until I was almost out of time.


## Essays
While AI can most definitely be utilized to help with generating content, ideas, and more, most essays I have written within this class did not utilize ChatGPT. Most of these essays were too full of my own personal experiences and opinions that I felt using AI would only get in the way of my writing. Having said that, I did use ChatGPT in this essay. More specifically, I asked ChatGPT to help me get a broader perspective on traditional learning and modern learning so that I can think about and compare to. I also asked about AI’s practical applications as my personal knowledge is less than favorable at the moment.


## Final Project
In the creation of our final project, I asked AI for help in making certain things that I have concepts for but never actually coded or implemented before. For example, our site deals with users looking at recipes and we wanted the users to be able to click a favorites button on a recipe they like and I know how to work with the button but I am not sure as to how I save them to a user's home page. So, I asked ChatGPT on how I might go about creating a button that has this feature in js code and it replied with one code method and an explanation of the code. I then told it "Make it so that each user has their own array of favorites" and it changed the button handle to this: 
```
  const handleFavoriteToggle = () => {
    if (isFavorite) {
      // Recipe is already favorited, remove the current user from the owner array
      const existingFavorite = recipeInfo.find(item => item._id === recipe._id);
      const newOwner = existingFavorite.owner.filter(owner => owner !== userEmail);
      console.log(newOwner);
      Recipes.collection.update(
        { _id: existingFavorite._id },
        { $set: { owner: newOwner } },
        (error) => {
          if (error) {
            // console.error('Update Error:', error);
          } else {
            console.log('Item updated successfully');
            // swal('Success', 'Item removed from favorites', 'success');
          }
        },
      );
    } else {
```
After a few more prompts to fix the bugs and error, I finally had a functional favorite button!


## Learning Concepts / Tutorials
When it came to the use of AI for learning concepts and tutorials, this was not a common thing that I used it for. I felt that code academy and the other sites we used to learn Html and JavaScript and everything else worked well enough for a teacher, explaining and breaking things down when first learning them that it all made sense. I also wanted to avoid the use of AI because I wanted to ensure that I was properly learning the basics so that I would have a solid foundation for the rest of the semester to build off of. Also the idea of using ChatGPT to create or be used for tutorials was never a thought that occurred to me. I often forget just how much one can do with the powers of AI.


##  Asking Or Answering In-Class / Smart Questions
AI can most definitely be used to help answer student questions but I never used AI in any such manner. I personally felt that when I ran into a problem it was often a problem that was a result of something occurring outside of the frame of reference or specific code that I was observing. It is also just easier for other students or teachers to answer because they will usually already have an idea of what the problem might be as they may have run into a similar problem. The utilization of AI to ask questions is something that seems illogical to me. It is better and faster if you simply ask the problem yourself since you already know what the error is even if you can’t figure out why. You asking AI to give you another question is just weird to me but I guess that just means that I know how to ask smart questions.


## Examples, Explanations, Writing, & Documenting Code
Explaining code to peers or in discussions was a predominantly human-driven task. While AI could suggest explanations, the contextual understanding and effective communication was stronger when human to human. I would occasionally ask ChatGPT to produce code examples of things such as react or CSS of image and text alignments. When I do so it would produce different results that I could test and play with to see for myself how certain fields would visually affect the site. In other situations I would have the AI write a section of my code such as classes and objects of the jamba juices on the menu as specified in the given homework prompt to save time with these tasks. When they finished, their output would also include documentation of the code explaining what each part of the code does and where I would have to write my own code in.


## Quality assurance
Quality assurance tasks benefited from AI, especially in identifying syntax and sometimes logic errors such as parameters for underscore methods errors or suggesting fixes. However, these would require the partial inputting of the assignment prompt to understand when needed. Some of the deeper issues  often required human expertise. AI was never necessary to fix ESLint errors as most of these errors were easily understandable for me and fixable through ESLint anyway.


# Impact on Learning and Understanding:
The incorporation of AI in my ICS 314 class has significantly influenced my learning experience. AI technologies have served as valuable tools for quick references, code generation, and ideation. They have enhanced my comprehension by providing alternative perspectives and approaches to problem-solving. The rapid assistance offered by AI has improved my efficiency in grasping new concepts and tackling coding challenges. On the other hand, it has caused me to become too comfortable with not knowing enough information as I can always ask the AI to remind me of it. This causes a reliance on it, stunting curtain growth of skills that by now would have fully grown.


# Practical Applications:
Beyond ICS 314, AI has a plethora of practical applications in real-world projects and collaborative activities. In initiatives like the Hawaii Annual Code Challenge (HACC), AI tools can assist in data analysis, code generation, and ideation. In our HACC project we used to understand how to implement a translation option for the whole page. The effectiveness of AI applications in addressing real-world software engineering challenges lies in their ability to augment human capabilities and streamline complex tasks. I have seen people on the internet use ChatGPT to fill in game codes where the users are inexperienced with no sense of direction but a solid goal in mind that leads to the incredible game existing.


# Challenges and Opportunities:
The biggest challenges and limitations that I observed while using ChatGPT in software engineering is that it can only help well with more contained common problems. What I mean by that is if you ask ChatGPT to work with or write code that is supposed to be connected with a multiple of pages, files, etc. then it runs into more problems when you try to attach everything together. It does not have access to everything, it only knows what you give it, so it is better to start small and build off what it gives you, making sure to test it as you go along. Another limitation that it has is that when working with uncommon application languages they are often too specific for ChatGPT to give you correctly syntactic code. Opportunities that arise from the use of AI are personalized learning paths where the AI can adapt to your strengths and weaknesses, optimizing your learning journey. I can also play a pivotal role in refining and adapting curriculums based on industry trends, emerging technologies, and the evolving needs of the software engineering field to ensure that education remains relevant in this ever-changing field.


# Comparative Analysis:
When traditional teaching methods are compared to AI-enhanced ways, AI shines in terms of offering quick references, code suggestions, and varied problem-solving viewpoints. Traditional approaches, on the other hand, provide a more thorough understanding, human engagement, and tailored feedback. The best strategy is a well-balanced integration that uses AI to boost productivity while maintaining a solid foundation using conventional techniques.


# Future Considerations:
Future developments in personalized learning, adaptable curriculum design, and more advanced AI technologies customized to the difficulties of software development look promising for the use of AI in software engineering education. Developing AI models for complex understanding and handling ethical issues are challenges. A smooth integration of AI and traditional methods of teaching will be possible with more studies and advances into the integration of AI in education.


# Conclusion:
The integration of AI, notably ChatGPT, in ICS 314 has greatly expedited learning through swift problem-solving and code generation. However, a caveat exists in the risk of overreliance, potentially impeding independent problem-solving skills. Challenges encompass limitations in handling larger code projects and uncommon languages. On the flip side, opportunities emerge in the form of personalized learning paths and refined curricula. Future courses should strike a balance between AI and traditional methods, refining AI capabilities, and addressing ethical considerations for an optimal and dynamic learning environment.

