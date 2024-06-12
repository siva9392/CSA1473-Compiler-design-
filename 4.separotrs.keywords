%{
#include<stdio.h>
%}
%%
if|else|while|int|switch|for|char { printf("\n%s is a KEYWORD", yytext);}
[a-zA-Z0-9]+ { printf("\n%s is IDENTIFIER", yytext);}
%%
int yywrap( ){}
int main()
{
	yylex();
}
   OUTPUT
   C:\Users\sivas\OneDrive\Desktop\program>flex identi.l

C:\Users\sivas\OneDrive\Desktop\program>gcc lex.yy.c

C:\Users\sivas\OneDrive\Desktop\program>a.exe
23

23 is IDENTIFIER
abc

abc is IDENTIFIER
%%
%%
"siva"
"
siva is IDENTIFIER"
include

include is IDENTIFIER
int

int is a KEYWORD
