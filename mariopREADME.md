#include <stdio.h>
#include <cs50.h>

void draw(int height);

int main(void)
{
    int height;
    printf("height: ");
    scanf("%i" , &height);
    
    draw(height);
} 

void draw(int height)
{
    if (( height -1) !=0 )
    {
        draw(height - 1 );
    }
    
    for (int i = 0; i < height; i++)
    {
        printf("#");
    }
    printf("\n");
}
