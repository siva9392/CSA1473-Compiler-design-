%{
#include <stdio.h>
#include <stdlib.h>

void validate_email(const char* email) {
    printf("Valid email address: %s\n", email);
}

void invalid_email(const char* email) {
    printf("Invalid email address: %s\n", email);
}
%}

%%

[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,} {
    validate_email(yytext);
}

.|\n {
    invalid_email(yytext);
}

%%

int main() {
    printf("Enter an email address to check its validity:\n");
    yylex();
    return 0;
}

int yywrap() {
    return 1;
}
