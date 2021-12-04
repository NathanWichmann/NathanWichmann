### Hi there 👋

<a href="https://nathanwichmann.github.io/My-App/">New React Portfolio</a>
- 🔭 I’m currently working on the Harvard CS50 class and finishing up the Complete beginners guide to C programming.
- 🌱 I’m currently learning the C programming language.
- 👯 I’m looking to find a position as a Junior Full Stack web Developer now as I have recently graduated from the Full Stack Web Developer program at Carleton University.
- 🤔 I’m looking for help with landing that position where I can learn all thats required to become a succsessfull Junior Developer.
- 💬 Ask me about my interests in coding. 
- 📫 How to reach me: email nathanwicker@hotmail.com, nathanwichmann12@gmail.com
- 😄 Pronouns: he/him
- ⚡ Fun fact: Coding bootcamp was fun and hard work, but it left me with more questions than answers, so I decided to go back to the beging and learn C.

// Example program #1 from Chapter 27 of Absolute Beginner's Guide
// to C, 3rd Edition
// File Chapter27ex1.c
/* The program gets the bookInfo structure by including bookInfo.h
and asks the user to fill in three structures and then prints them.
*/
//First include the file with the structure definition
#include "bookinfo.h"
#include <stdio.h>
main()
{
int ctr;
struct bookInfo books[3]; // Array of three structure variables
// Get the information about each book from the user
for (ctr = 0; ctr < 3; ctr++)
{
printf("What is the name of the book #%d?\n", (ctr+1));
gets(books[ctr].title);
puts("Who is the author? ");
gets(books[ctr].author);
puts("How much did the book cost? ");
scanf(" $%f", &books[ctr].price);
puts("How many pages in the book? ");
scanf(" %d", &books[ctr].pages);
getchar(); //Clears last newline for next loop
}
// Print a header line and then loop through and print the info
printf("\n\nHere is the collection of books: \n");
for (ctr = 0; ctr < 3; ctr++)
{
printf("#%d: %s by %s", (ctr+1), books[ctr].title,
books[ctr].author);
printf("\nIt is %d pages and costs $%.2f", books[ctr].pages,
books[ctr].price);
printf("\n\n");
}
return(0);
}

