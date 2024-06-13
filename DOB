%{
#include <stdio.h>
%}

%%
[0-9]{4}-([0][1-9]|1[0-2])-([0-2][0-9]|3[0-1]) {
    printf("Valid DOB: %s\n", yytext);
}

.|\n ;

%%

int main() {
    yylex();
    return 0;
}
