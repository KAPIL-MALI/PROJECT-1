# PROJECT-1


#include<stdio.h>
#include<stdlib.h>
#include<time.h>

int main(){

int RANDOM_NUMBER , GUESS , NUMBER_OF_GUESSES = 0;

srand(time(0));
RANDOM_NUMBER = rand() %100 + 1;

do{
    printf("GUESS A NUMBER BETWEEN 1 TO 100! \n");
    scanf("%d",&GUESS);

NUMBER_OF_GUESSES++;

if(GUESS > RANDOM_NUMBER){
    printf("LOWER NUMBER PLEASE! \n");
}
else if (GUESS < RANDOM_NUMBER){
    printf("HIGHER NUMBER PLEASE! \n");
}
else{
    printf("CONGRATULATIONS !! YOU HAVE GUESSED THE RIGHT NUMBER IN %d ATTEMPTS .",NUMBER_OF_GUESSES);
}

}while(GUESS != RANDOM_NUMBER);

return 0;
}
    
