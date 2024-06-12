%{
int vcount=0;
int ccount=0;
%}
%%
[aeiouAEIOU] {vcount++;}
[a-z,A-Z] {ccount++;}
%%
int yywrap(){}
int main()
{
printf("enter the string with vowels and consonants:");
yylex();
printf("\n no of vowels ::%d \n",vcount);
printf("\n no of consonants ::%d \n",ccount);
}

      OUTPUT:

C:\Users\sivas\OneDrive\Desktop\program>flex cons.l

C:\Users\sivas\OneDrive\Desktop\program>gcc lex.yy.c

C:\Users\sivas\OneDrive\Desktop\program>a.exe
enter the string with vowels and consonants:siva sankar is a good boy

^Z

 no of vowels ::9

 no of consonants ::11
