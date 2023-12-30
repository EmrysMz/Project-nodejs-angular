# Project-nodejs-angular

# ( Open the BUILD.md file in the repository to know how to setup the application !!!) 

## Introduction

Hello, this is our final project for the node & angular course at ESILV. Our project is named Cerebralize and it's a learning web application like Anki that gives the possibility to study flashcards already implemented or created by the user himself. It uses the time-spaced learning method to improve the learning process.

The Cerebralize learning application offers a user-friendly interface for an optimal learning experience. Upon entering the home page, users encounter a top navigation bar featuring buttons like "explore lessons," "study now," and "progress statistics," providing a seamless management system for learning packages.

In the "explore lessons" section, users can effortlessly discover pre-existing packages with detailed information, including a package's name, description, category, target audience, and difficulty level. For example, by selecting "physics lessons," users can access flashcards that present questions and hidden answers, enabling them to add pertinent facts to their personalized learning deck.

Transitioning to the "study now" section, users gain insights into their deck's content, package associations, and study details. Clicking on a specific course, such as "physics course 3," reveals flashcard content. Users can fine-tune their study schedule by assigning confidence levels and marking completion when confident.

The "progress statistics" feature provides a comprehensive overview of the user's learning journey, offering detailed insights into package progress and fact statuses. Users can view start dates and estimated end dates based on package difficulty.

Furthermore, Cerebralize empowers users to create their own packages and facts, allowing for a personalized learning experience. Users can easily add learning content to custom packages, edit existing facts and packages, or delete them as needed.

Cerebralize ensures a versatile and user-centric platform for effective learning management.

## Plan and interfaces

The plan of our web application is the following : 

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/53a673bf-3549-473a-af2d-23cbe18e8759)


Now we're going to show you how to use our app.

When you access on the website, this is the first page :


![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/1d3c3b78-9f83-40e3-907e-a2af65d4bdaa)

Just click on the button and you can select an already existing user in the dropdown menu, this is for the demonstration to show different users since we can't create authentication systems for this project.


![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/3ee53138-876c-4db5-a8fb-5eb37d521957)

Then click on the start button :

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/40664458-a556-41bd-823b-ab6b86c675eb)

You get on the user's home page as you can see : 

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/ed36575b-a579-40ae-90e0-056ec74dbc1e)

From this page, you can see that there is a navigation bar on the top. There are several buttons like :

- Home ( to return to this homepage)
- Explore Lessons (To get all existing packages from the database)
- Study Now (To study facts in the user's deck)
- Progresses Statistics (To display the progression of the user)
- Add ( To add learning packages and facts)
- Update ( To edit learning packages and facts)
- Delete ( To delete learning packages and facts)

Let's begin with the Explore Lessons page : 


![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/97312952-a5c9-4408-962c-8ef3ef47adf5)

In this page you can see various learning packages with their title, category, description, target audience, difficulty. Some of them were introduced directly in the database and others were put using the application.

You can click on the "Discover Learning Facts" button below a learning package card to display the learning facts within : 

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/310a93dc-c464-4b10-89c5-e4e505bba3da)

On this page you can see the differents learning facts into a learning package. You can see the content by clicking on the start green button:

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/c6622ccd-b5d6-4eb7-abee-3396e7ad79da)


The content is like a flashcard, you have a title, a description and a question with it's answer. You can see the answer by clicking on the show answer button.

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/bb068894-a78b-4e09-9e4d-4f43ca894425)


If the user wants to work another time on this course he can add it to his deck by clicking on the "Add to my deck" button.


Now, let's move on the "Study Now" menu. On this page you can see all the facts on a user deck grouped by package:


![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/90efa6b7-58ba-43d6-be5d-97e8fc3ab5fa)


You can see the status of each learning fact, if it's finished or no or the next time to study. You can study a fact by clicking on the button "Go to fact":


![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/33e706d9-c10d-4e56-ad65-dc3b0dc0472a)


Here you can study the fact and if you want yo study it again just enter your confidence level from 1 to 10 to get the next study time. If you master the fact you can click on "Complete Learning".

Next, we have the "Progresses Statistics" page where you can see informations about the completion of the courses:



![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/4e44b8a2-8389-47e2-8788-b20100e2c58e)

We used highcharts to display the numer of times that a user reviews a course.

It can make dynamic plots like this one : 


![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/ce50a158-fef2-498b-be79-c70e3998ee9f)

Let's see how to create a learning fact and a learning package. Since a learning fact is inside a learning package, you have to create the learning fact after creating the learning package if it's a new.


![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/ab4ce7f9-9c3b-40e7-8750-fe022b838c8e)


Fill the form, select the package and click on submit

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/cb3131ae-c893-4fb1-b0b2-f64f11bebf00)

We can see the newly added learning fact : 


![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/62584cab-92ec-4515-aed4-4d0bcec78441)


It's basically the same thing for packages :

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/5eadbf97-3a2f-4625-9169-e05faa35893f)

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/ab0ad660-229b-4576-bd62-236ce95a8bcb)



We can also edit learning packages and learning facts :


![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/998420b6-ce23-4513-be2a-1ce2d9617b4e)

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/1203d99c-b7a7-4efc-946c-d260cf9e0c39)

And finally we can also delete learning facts :

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/2a2fb3d6-8ff5-4d31-b9d9-7d5694ffb8e2)

![image](https://github.com/EmrysMz/Project-nodejs-angular/assets/131869495/ee08b475-2df1-4f0c-81aa-c48476270c58)


