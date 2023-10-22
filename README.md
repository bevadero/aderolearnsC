# aderolearnsC
C portfolio

// bevadero
// 22/10/2023

// a function fullName that:
// asks the player for a first name,
// asks the player for a last name,
// concantenates the last name to the first name,
// prints out the player's full name on the screen.

#include <stdio.h> 
#include <string.h>

// a function fullName that:
void fullName() 
{ 
    char firstName[42], lastName[42], bothNames[70]; 
    
    // asks the player for a first name,
    printf("What is your first name?\n");
    scanf("%s", firstName); 
    
    // asks the player for a last name,
    printf("What is your last name?\n");
    scanf("\n%s", lastName); 
    
    // concantenates the last name to the first name,
    strcpy(bothNames, firstName);
    strcat(bothNames, " ");
    strcat(bothNames, lastName);

    // prints out the player's full name on the screen.
    printf("Your full name is %s.\n", bothNames); 
} 

int main() 
{ 
    // call the fullName function
    fullName(); 
    
    return 0;
} 
