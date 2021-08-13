# Bobae Match

By Justin Wong

## Table of Contents
* [What is BobaeMatch?](#what)
* [Application Architecture & Technologies Used](#tech)

## <a name="what"></a>What is BobaeMatch?

BobaeMatch is a fullstack web dating application that connects users based on their favorite boba tea interests such as: drink addons, sugar levels, tea choices and more. 

Users start off by creating a profile and specifying their favorite boba tea customizations through a series of guided choices as they create their account. These preferences can also be changed by editing their preferences on their profile page.

Once the user's preferences are set, the user is then able to search for matching users with similar boba tea tastes in the find bobaes section of the website. Here the user will be able to see other users profiles and either press on the heart icon to match with the other user or press on the broken heart icon to reject matching with the other user.

If users have matched with each another on both their accounts, they will be able to see each another on the current matches page where they will be able to chat through the messenging system located on the bottom right of the page. On the current matches page, users will also be able to delete their matches in the event their pairing does not work out.

### Here is BobaeMatch at a glance with a demonstration account:

## <a name="tech"></a>Application Architecture & Technologies Used

BobaeMatch's fullstack framework consists of a back-end that incorporates Python, Flask, SQLAlchemy, and a Postgres data base. The front-end framework consists of JavaScript, React, and Redux. 

Users interact through Bobaematch's front-end which displays our React UIs and requests data from the back-end or dynamic data that is pre-rendered and accessible through the browser from the Redux store, which also dispatches requests to the back-end to display changing data without page refreshes.

Additional technologies that were incorporated include: 
* Amazon Web Services (AWS) to allow users to upload their profile pictures and use them on our site
* WebSockets for the messenging application so users can chat live with one another.

## Custom Courasel Code Snippet
BobaeMatch includes a custom courasel on the home page as I did not want to follow guides or code online but rather create the component myself. My version of the courasel uses setTimeouts and Rerenders to swap image components, and only uses 2 components for this process. These two components can iterate through any series of images and efficiently display them on the page.

![](https://github.com/Sirpeter89/MatchMyBoba/blob/main/customcourasel.PNG)

## Querying Algorithm Code Snippet
I relatively found working with the backend pretty interesting and learned a good amount about SQLAlchemy queries in this process. Working with the code was a fun learning experience and this was the main functionality of my program.

![](https://github.com/Sirpeter89/MatchMyBoba/blob/main/queryexample.PNG)

The heart of BobaeMatch resides in the query for matches, at the moment the querys are relatively simple as they query users by an interest and if there aren't enough users we go down the list to the next interest. This also includes whether the users are lactose intolerant, since that may be an ideal match, or if they like fruit teas.

## Future Plans and Interest
Creating BobaeMatch was an enticing yet difficult journey. Throughout the trials I learned a lot about managing the backend and data queries, yet at the same time styling was a big challenege but I really enjoyed my time creating my own components that some prefer using apis for. Although I do not hate the notion of apis, I used this project as my own opportunity to learn and create things from scratch.

Future implementations include adding a messaging feature, possibly google maps, and amazon webservices for my images.
