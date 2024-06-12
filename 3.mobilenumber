%%
[1-9][0-9]{9} {printf("\nMobile Number Valid\n");}
.+ {printf("\nMobile Number Invalid\n");}
%%
int main()
{
	printf("\nEnter Mobile Number : ");
	yylex();
	printf("\n");
	return 0;
}
int yywrap()
{ } 

OUTPUT:

C:\Users\sivas\OneDrive\Desktop\program>flex number.l

C:\Users\sivas\OneDrive\Desktop\program>gcc lex.yy.c

C:\Users\sivas\OneDrive\Desktop\program>a.exe

Enter Mobile Number : 9392731584

Mobile Number Valid

