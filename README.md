# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include<stdio.h>
int main(){
    int a=44;
    a=a<<3;
    printf("After Left Shift Operation value of a is:%d",a);
}
```

## OUTPUT
![shift](https://github.com/user-attachments/assets/3f3118ab-5cc7-4378-aa43-c5fe1dab90ae)










## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```

#include<stdio.h>
int main()
{
    int a,b;
    scanf("%d%d",&a,&b);
    if(a==b)
    {
        printf("X is equal to Y");
    }
    else
    {
        printf("X is NOT equal to Y");
    }
    return 0;
}

```


## OUTPUT
![same](https://github.com/user-attachments/assets/fa378f57-35ec-4f33-8b4b-f154ac100841)

![diff](https://github.com/user-attachments/assets/9f7fc31f-9a20-4f55-9661-0a11a6e268f7)

           
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <ctype.h>

int main() {
    char str[100];

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    for (int i = 0; str[i]; i++) {
        str[i] = tolower(str[i]);
    }

    printf("Lowercase string: %s\n", str);

    return 0;
}
```

## OUTPUT
![lowercase](https://github.com/user-attachments/assets/e791467c-caff-4b91-96fe-8eed17469be0)





## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    char str[100];
    int count = 1, i = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    do {
        if (str[i] == ' ') {
            count++;
        }
        i++;
    } while (str[i] != '\0');

    printf("Total number of words: %d\n", count);

    return 0;
}
```


## OUTPUT
![words](https://github.com/user-attachments/assets/f3009f19-c43a-4089-8ede-7a13b3fa3743)






## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    char c1[100], c2[100];
    int flag = 0, i = 0;

    printf("Enter the first string: ");
    scanf("%[^\n]", c1);
    getchar(); // To consume the newline character left by scanf

    printf("Enter the second string: ");
    scanf("%s", c2);

    while (c1[i] != '\0' && c2[i] != '\0') {
        if (c1[i] != c2[i]) {
            flag = 1;
            break;
        }
        i++;
    }

    if (flag == 0 && c1[i] == c2[i]) {
        printf("Strings are same\n");
    } else {
        printf("Strings are not same\n");
    }

    return 0;
}
```


## OUTPUT
![same strng](https://github.com/user-attachments/assets/c1c71981-63d6-43c6-bfe1-14a6e64baf00)

 

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

