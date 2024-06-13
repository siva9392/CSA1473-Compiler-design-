%{
#include <stdio.h>
#include <stdlib.h>

void validate_url(const char* url) {
    printf("Valid URL: %s\n", url);
}

void invalid_url(const char* url) {
    printf("Invalid URL: %s\n", url);
}
%}

%%
(http|https)://[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}(/[a-zA-Z0-9._%+-]*)* {
    validate_url(yytext);
}

.|\n {
    invalid_url(yytext);
}

%%

int main() {
    printf("Enter a URL to check its validity:\n");
    yylex();
    return 0;
}

int yywrap() {
    return 1;
}
