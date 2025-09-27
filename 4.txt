#include <stdio.h>

void main() {
    char first_choice;
    char second_choice;

    printf("----------Online Food Ordering System----------\n");
    printf("Select a category, Fast Food or Drinks(Enter F for Fast Food and D for Drinks): ");
    scanf(" %c", &first_choice);

    switch (first_choice)
    {
    case 'F':
        printf("B: Burger\nF: Fries\n");
        printf("What would you like to order: ");
        scanf(" %c", &second_choice);
        switch (second_choice)
        {
        case 'B':
            printf("Burger Ordered!");
            break;
        
        case 'F':
            printf("Fries Ordered!");
            break;
        
        default:
            printf("Invalid Input, Kindly enter B or F.");
            break;
        }
        break;
    
    case 'D':
        printf("S: Soft Drink\nC: Coffee\nT: Tea\n");
        printf("What would you like to order: ");
        scanf(" %c", &second_choice);
        switch (second_choice)
        {
        case 'S':
            printf("Soft Drink Ordered!");
            break;
        
        case 'C':
            printf("Coffee Ordered!");
            break;
        
        case 'T':
            printf("Tea Ordered!");
            break;
        
        default:
            printf("Invalid Input!");
            break;
        }
        break;
    
        default:
            printf("Invalid Input, Kindly input F or D.");
            break;
    }
    
}