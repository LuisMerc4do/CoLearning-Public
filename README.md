# CoLearning

## At the moment I am in talks according the first implementation of Colearning
# What is CoLearning?


CoLearning is a free online technology learning platform designed to reduce educational inequalities and offer new growth opportunities to all Colombians. CoLearning represents a new way of thinking about education, prioritizing the learning of emerging technologies and their application in solving real-world problems. Additionally, it fosters innovation and entrepreneurship by providing students with the necessary tools to turn their ideas into concrete projects.

# https://colearning.vercel.app
# Why CoLearning?


In Colombia, many students in lower-middle-class schools face challenges such as drugs, violence, and lack of educational resources, which hinder their academic progress. Education in areas like programming, data analysis, and computing is practically nonexistent in the current educational system. This lack of computational learning means that there are no free and accessible alternatives for students to acquire these crucial skills. The lack of promotion of technological knowledge is evident: very few students know how websites are developed or that there is an engineering field dedicated to it.

# How can CoLearning help?
CoLearning is designed to address these challenges in several ways:

- Access to Quality Education: We provide free and accessible courses in programming, data analysis, and other technologies, eliminating economic and geographic barriers.

- Practical Application of Knowledge: Our courses are designed for students to apply their knowledge to real-world problems, fostering practical and relevant skills for the job market.

- Innovation and Entrepreneurship: CoLearning encourages innovation and entrepreneurship by providing resources and mentorship for students to develop their own ideas and projects.

- Safe and Enriching Environment: By creating an online learning community, we keep students away from dangerous environments and offer them a safe space to develop and learn.

- Knowledge and Awareness: Through our courses, students will discover the various opportunities technology offers, from website creation to software engineering, expanding their horizons and professional aspirations.

CoLearning not only offers an educational platform but also builds a bridge to a better future, where all Colombians can access the opportunities that technology provides and improve their quality of life.


# DEVELOPMENT 
### Technologies used: NEXTJS, REACT, TAILWINDCSS, PRISMA, POSTGRESQL, AUTHJS 5, SHADCNUI

# Before you Continue... 
You might be wondering why you used a full-stack "environment” like Nextjs when is a better long-term solution to having a separate backend, well, for adaptability, usability, and easy implementation. I don't discard the option of having a separate backend for some of the functionalities of the app but right now I consider that the requirements of the app are completely fulfilled by using next.js

## So Why Next.Js without a backend? 
Well, my app is mostly repetitive tasks and doesn’t need to use a huge amount of data, the response times are
not necessarily long, fetching courses, user information, and chapter information is not a big deal in terms of needing an special and elastic backend server for this. Yes I am thinking about expanding my app but for what I need now and my target requirements, Next.js stands as the best option. 
### Sorry for the mix of spanish and english, the code is all in english but the webpage is in spanish so at the moment of writing the text my brain gets crazy.
## Chapter page 
## Coding Excersice Chapter Page
![image](https://github.com/user-attachments/assets/ac4825c9-b1a8-44eb-b568-5aecbd32ee3a)
![image](https://github.com/user-attachments/assets/92910e58-78a6-47a0-ba09-ae25f6439414)
### output checking the expected output 
![image](https://github.com/user-attachments/assets/7d2b4624-14cf-4473-93b7-4d3ec981a56e)
### menu with all the chapters and working to implement sections
![image](https://github.com/user-attachments/assets/08de133c-30ab-430f-86da-4f06b4abcc70)

## Course setup 
![image](https://github.com/user-attachments/assets/fa3cb288-af35-4dda-89f1-acf605b106c5)
![image](https://github.com/user-attachments/assets/79a2ac35-2aaf-4707-9471-592655bb99b3)
![image](https://github.com/user-attachments/assets/5d8cb172-2435-41f9-a655-008d14f18754)
### CodeChapter is optional. We also have the option of video chapter
![image](https://github.com/user-attachments/assets/cd7cc751-dc37-40c9-82ef-7ecfcf9067ed)

### This is the end of Initial structure, I didn't track my process step by step of my development until here, I do have my github commits with all the descriptions but not organized in a changelog like this.
# update 16-07 Implementation of authjs 5
### Was a bit challenging Authjs is a consistent way to authenticate the user with nextjs but the documentation is a bit unclear at the moment, I had to watch many videos in youtube and stackoverflow to properly implement it.

# update 17-07 Moving from api endpoints to server actions for best nextjs 15 integration

The whole thing with server actions is paradigm changer, I used to work with react but usign a separate backend, asp.net or node.js, usign the typical endpoints, fetching an endpoint and getting a response back, now with nextjs everything is different now we have something called served actions which is basically the usage of backend and frontend in the same environment, so basically you can have a server action, this works like an object (it looks like any other tsx or js function) you can fetch a table of courses and returning all the courses. And basically the main point of this is that you can call that server action in your server component and work with that data straight away without needing to fetch any endpoint. It's so easy to work like this. You have to focus most in the logic and how to fetch, protect and avoid leaks thank properly fetching and conecting backend with frontend. And I'm telling you I used to work with asp.net and react, I know about problems while connecting back with front.

## So it looked a bit like this before


![image](https://github.com/user-attachments/assets/04bd186e-21b3-4c22-bd99-342fa62f1657)


![image](https://github.com/user-attachments/assets/30b6689c-9a8b-4fd2-b537-e8fa7e3df43e)



## Now it looks like this


![image](https://github.com/user-attachments/assets/503e1cdd-783a-420b-99e4-e57c452bb22e)


![image](https://github.com/user-attachments/assets/c4670dfa-f00b-4a16-88bd-6af782fbea92)

# update 19/07

I worked more on the implementation of the login and signup page, usign jwt for the authentication token, ensuring more security for each account avoiding data leaks. Right now the design is just a template from the shadcn page but the functionality of signup and login is mostly done. I thought about email or mobile verification but my audience is not very used to it so i'll find other alternatives to avoid spams like captcha or something like that. 


![Captura de pantalla 2024-07-21 114222](https://github.com/user-attachments/assets/0e502e57-3d2b-46af-bdd4-8464680991c5)
![Captura de pantalla 2024-07-21 114211](https://github.com/user-attachments/assets/6c80fdee-6a35-4e5b-9942-ab88bebaf04f)



# update 21/07

I have been working on the course page for the past few days, the text is completely functional and it fetchs the data from the database. I have watched some inspiration for the brand design and how can i build the webpage, here are some updates: 

![Captura de pantalla 2024-07-21 121407](https://github.com/user-attachments/assets/dd282741-4b87-4466-a33c-7e7862ba06b4)

# update 22/07

I worked a bit on the main hero page, I put some animations usign Magic UI, i'm planning to use framer motion for a few more things in the future, i'm planning to make the webpage as much efficient as possible, even my Nokia 1990 will run it.  And yes I know i need to animate the cartoon as well, but I'm still thinking about it.

![Recording 2024-07-21 at 12 32 58](https://github.com/user-attachments/assets/334debe5-2ec0-428a-83a3-29b83260e9a0)

# update 22/07 
Okay today is weekend so I don't have to work, i've been working on the course page, I recon that I spent more time thinking about the design than actually coding it. I like the form is taking, very modern. 

![Recording 2024-07-21 at 15 33 27 (1)](https://github.com/user-attachments/assets/8ccde73b-704b-4b00-87e0-a8e8c5fdd9c2)

# update 23/07 

I am working now on the login page, the design and header is still in progress, I'm still considering new options for the general design and personality of the webpage, until then I'm focusing on the main functionalities for early deployment. Is not that I don't like the design I'm usign now is just that I don't really know if it's the best I can do for a project like this. I feel like i need something more engaging. Oh btw I removed the container on the header. I just feel like doing it.

![Captura de pantalla 2024-07-24 175125](https://github.com/user-attachments/assets/25352fac-3ca0-461e-815e-a2f2414dbeda)

# update 24/07


I am also working on the header, I already implementated a different header when user is logged in, with an avatar component from shadcn and a dropdown menu, it's already connected with the db so 0 problems. I started working on the control panel and i need to implement the idea I have for the login to not think about authentication and user control for a while and focus on finishing the main functionalities for courses. 

![Captura de pantalla 2024-07-24 175555](https://github.com/user-attachments/assets/37efa6f3-8ed9-4bed-9529-840157f8f3c4)

# update 25/07

I spent the whole day trying to create a design I like in figma with background animations and all of that stuff but I didn't like anything so basically I waste part of my day, I don't want to continue with secondary functionalities until I have a predefined idea of what i want to create in terms of design, I'm getting there, one day at a time. I'm not frustrated, on the other hand, I implemented the course information that will be shown in the course page. I didnt have this functionality before so yeah. 


![Captura de pantalla 2024-07-25 200633](https://github.com/user-attachments/assets/a24c82b7-289d-4386-b54b-36d7ca71fb7f)

# update 26/07 

So, Today is friday, I decided to work a bit on the course page, change a few things I didn't like enough so this is the result, with this I feel that the whole page in general is taking a good shape, I have to implement a few more things to make it look better:

![Captura de pantalla 2024-07-27 173108](https://github.com/user-attachments/assets/731d24b8-bf94-4eaa-ae46-90d43b54c975)

# update 27/07 

I spent the whole day working on the code chapter page. And I am very proud of myself, it wasn't easy, I changed from monaco to code mirror, I redesigned the whole page and I think right now is completely functional, I just need to change the navbar and add a few more details.


![Recording 2024-07-27 at 17 21 02](https://github.com/user-attachments/assets/25c95935-720b-41ea-a456-7a6fd606443c)


# update 29/07

I couldn't work on the project yesterday, but today i feel more motivated than ever, finally I found colors I like, I feel like I will put the dark mode as the main mode, It's just more apropiate the coding environment with dark colors 

![Captura de pantalla 2024-07-29 212421](https://github.com/user-attachments/assets/1382bd41-7ea6-4ef7-aca7-1f03ce1bdc2b)

# update 31/07

After a few changes I am going to leave the ide like this and I will focus on other things, at the moment I think this is good enough. 


![IDEColearning](https://github.com/user-attachments/assets/2c506c1a-c1fa-424f-a833-183e9659d47d)
