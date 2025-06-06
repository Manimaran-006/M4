
# Name:Manimaran V
# Reg.no:212224220060
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
    #include<stdio.h>
    int main() 
    {
    int a=44,b=3;
    int res;
    res=a<<b;
    printf("Result after left shifting %d by %d positions = %d\n",a,b,res);
    return 0;
    }
## OUTPUT

![Screenshot 2025-04-28 171734](https://github.com/user-attachments/assets/1b1dc65e-857b-4ec2-9046-a2178f5673cf)

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
    #include<stdio.h>
    int main()
    {
	int a,b;
	printf("Enter two numbers:\n");
	scanf("%d%d",&a,&b);
	if(a==b)
	{
		printf("Both are equal");
	}
	else
	{
		printf("Both are not equal");
	}
    }

## OUTPUT

![Screenshot 2025-04-28 172105](https://github.com/user-attachments/assets/f8835c88-741a-41f3-a8c8-7a2a76d323c5)

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
    #include<stdio.h>
    #include<ctype.h>
    int main()
    {
    char str[100];
    int i;
    printf("Enter a string:\n");
    scanf("%s",str);
    for(i=0;str[i]!='\0';i++)
	{
        str[i]=tolower(str[i]);
    }
    printf("Lowercase string: %s\n",str);
    }
## OUTPUT

![Screenshot 2025-04-28 172416](https://github.com/user-attachments/assets/7c43460a-97a8-46c1-afa3-bf9d546f4e7e)

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
    #include<stdio.h>
    int main()
    {
    char str[200];
    int i=0,count=1;
    printf("Enter a string:\n");
    fgets(str,sizeof(str),stdin);
    do 
	{
        if(str[i]==' '||str[i]=='\t')
		{ 
            count++;
        }
        i++;
    } while(str[i]!='\0'&&str[i]!='\n');
    printf("Total number of words=%d\n",count);
    }
## OUTPUT

![Screenshot 2025-04-28 172709](https://github.com/user-attachments/assets/a37f7f29-61a5-43ea-9cc4-737e878d2fe6)

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
    #include<stdio.h>
    int main()
    {
    char c1[100],c2[100];
    int i=0,flag=0;
    printf("Enter the first string:\n");
    scanf("%[^\n]s",c1);
    printf("Enter the second string:\n");
    scanf("%[^\n]s",c2);
    while(c1[i] != '\0' && c2[i] != '\0') 
	{
        if(c1[i]!=c2[i])
		{
            flag=1;
            break;
        }
        i++;
    }
    if(c1[i]!='\0'||c2[i]!='\0')
	{
        flag=1;
    }
    if(flag==0)
    {
       printf("Strings are same\n");
    }
    else
    {
       printf("Strings are not same\n");
    }
    }

## OUTPUT
 
![Screenshot 2025-04-28 173321](https://github.com/user-attachments/assets/a3599713-beb9-418f-ac9a-fdab00bf4196)

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

