
#include <stdio.h>

int main() {
    float tr = 0, Price;
    int discount = 0, items;

    for (int i = 1; i <= 5; i++)
    {
        printf("Enter number of items for customer %d: ", i);
        scanf("%d", &items);

        for (int j = 0; j < items; j++)
        {
            printf(" Enter price for item %d: ", j + 1);
            scanf("%f", &Price);

            tr += Price;
            if (Price > 100)
            {
                discount++;
            }
        }
    }

    printf("\nTotal Revenue: $%.2f", tr);
    printf("\nItems receiving a discount: %d\n", discount);
    return 0;
}
