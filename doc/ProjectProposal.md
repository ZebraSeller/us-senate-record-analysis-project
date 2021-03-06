# Project Proposal

## 1. Project Title

US Congressional Voting Record Analysis

## 2. Project Summary

In this project, the voting records of Senators from the 117th Congress (2021-2023) will be analyzed. This analysis will display the results of roll call votes over the duration of the 117th Congress. Users will be able to query this data in different ways, such as making categories based on Senator political parties and State origin, or looking at which roll call votes were favoured by certain parties. Users can also perform Create, Read, Update, Delete, and Search operations on the data, so that the the database can be constantly updated or corrected when inaccuracies are noticed. The user can also change the data to other datasets like the 116th congress.

The data set for this project consists of tables showing all Senators in the 117th Congress, roll call votes that have been voted on, the results of such votes, and the individual votes of Senators for each bill. Senators in the dataset can be identified by their distinct ICSPSR numbers, and roll call votes can be identified by their distinct roll call number. The votes of senators can be shown for each bill, with the following table explaining votes:

| Cast Codes | Description                                          |
| ---------- | ---------------------------------------------------- |
| 0          | Not a member of the chamber when this vote was taken |
| 1          | Yea                                                  |
| 2          | Paired Yea                                           |
| 3          | Announced Yea                                        |
| 4          | Announced Nay                                        |
| 5          | Paired Nay                                           |
| 6          | Nay                                                  |
| 7          | Present (some Congresses)                            |
| 8          | Present (some Congresses)                            |
| 9          | Not Voting (Abstention)                              |

## 3. Project Description

The problem we want to solve is that people may not be aware of how their senators vote, or what bills their party voted for or voted against. We will solve it by showing people the data corresponding to the votes, and analyze the data to show the users what their senators/party voted for.

The way we will accomplish this is by combining data from Senators, Senator bills, States, and political parties. People will then be able to query this data, and see a graph visualization of such data. This will be useful for seeing trends in the way Senators vote based on State and Party, for seeing the political parties that dominate certain States, and for maintaining a general up-to-date informative repository on the United States Senate.

## 4. Usefulness

The usefulness of the project is in showcasing a user friendly data set, with interactive options such as data querying and updating the data set.

Updating the data set can be useful for users trying to represent Senates from past or future years, while querying the data may allow users to see trends in the votes based on political parties or states. For example, a user would be able to see how Senators from their home state or political party vote on bills. Furthermore, the user can interact with the graph (creative component) to visualize a political map of the United States.

People can also become more informed regarding the bills voted on, based on the description of bills and the results of these bills (i.e. whether or not they passed or failed).

## 5. Realness

All the information about Senators, their states, and political parties comes from the [voteview.com](https://voteview.com/data) website. It represents real data for the current 117th Senate, showcasing their bill votes and political affiliations. We also manually get the image urls of the Senators from online resources.

The description of bills comes from the [senate.gov](www.senate.gov/legislative/LIS/roll_call_lists/vote_menu_117_1.html) website, and shows the date, result, and matter being voted on for each bill. We will convert the data as an xml file and convert it into a SQL database.

## 6. Functionality

We will be make a searching tool to display the votes of each senator. It can pull data of votes from a database, then visualize and analyze it.
The users can create, delete, update data in the database to make sure the data we have is accurate and up-to-date. They can also search for specific entries of data.
Data that will be stored for this project include:

1. every vote that occured in the Senate of the 117th congress
2. Senators' IDs, names, states, Photos(Maybe)
3. Information about the bills, what they are about, their results, their dates etc.
4. Parties and their members
   Basic functions of our web app include:
5. Search for vote data about specific senators, rolls, or parties etc.
6. Change/maintain the database by creating, deleting, updating data. For example, if the user notices any inaccuracy with the data, it can be corrected by deleting or updating the entry.
7. Summarize/Analyze the data requested by the user.

The creative component is to visualize the data, such as creating a pie chart, bar chart etc. to show the user the result. We plan to achieve this by using javascript/react, or other open-source libraries

## 7. UI Mockup

The project and data will be displayed using a website.
![image](https://media.github-dev.cs.illinois.edu/user/12602/files/019b4588-6ef6-4c57-ae0a-775666475fa2)
![image](https://media.github-dev.cs.illinois.edu/user/12602/files/193836dc-f164-4492-a7b3-c16c1526e68e)

## 8. Project Work Distribution

Moiz - Preapring the data, handling changes to the data, design the database model, setting up backend routes, designing advanced database program.
Boyang - Develop the frontend, try visualization (generating graphs), design the database model, setting up and maintaining the database, setting up backend routes.
Tuan - Preparing senate Roll Call Data, design the database model, designing advanced database program.
Minh - Preapring the data, Handle queries and Database, design the database model, setting up backend routes.
