#include <stdio.h>
#include <math.h>

void main() {
    float a, b, c, discriminant, real, img, root1, root2;
    printf("Enter value of a: ");
    scanf(" %f", &a);

    printf("Enter value of b: ");
    scanf(" %f", &b);

    printf("Enter value of c: ");
    scanf(" %f", &c);

    discriminant = (b * b) - (4 * a * c);

    if (discriminant < 0)
    {
        real = -b / (2 * a);
        img = sqrt(-discriminant) / (2 * a);
        printf("Roots are imaginary.\n");
        printf("Roots are %.2f + %.2fi and %.2f - %.2fi", real, img, real, img);
        
    }
    else
    {
        if (discriminant == 0)
        {
            root1 = -b / (2 * a);
            printf("Roots are real and equal.\n");
            printf("Both roots equal to %.2f", root1);
        }
        else
        {
            root1 = (-b + sqrt(discriminant)) / (2 * a);
            root2 = (-b - sqrt(discriminant)) / (2 * a);
            printf("Roots are real and distinct.\n");
            printf("Roots are %.2f and %.2f", root1, root2);
        }
    }
    
}