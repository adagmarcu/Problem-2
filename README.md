// Problem-2
#include <iostream>
#include <string.h>
#include <stdlib.h>

using namespace std;

int missingLetter(char text[])
{
int variable = (int)text[0];

variable = variable + 1;


for (int i = 1; i < strlen(text); i++)
{

   
    if (variable != text[i])
        return variable;

    else
    {
        variable = variable + 1;
    }
}
}

int main()
{
char text[28] = { 'd', 'e', 'g', 'h' ,'\0'};
int variable_aux = missingLetter(text);
cout << (char)(variable_aux );
cout << endl;

char text1[28] = { 'O','Q','R','S','\0' };
int variable1_aux = missingLetter(text1);
cout << (char)(variable1_aux);
}
