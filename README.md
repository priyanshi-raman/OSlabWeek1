# OSlabWeek1
Trying!
#include <stdio.h>
#include <string.h>
#include <stdlib.h>
int P;
struct menu{
int code;
char food[100];
int price;
}item[50];
FILE *kitchen;
FILE *bill;
void main()
{
    printf("Welcome to 4 seasons cafe!\nWe hope to serve you delicious and fresh food!\n");
    printf("Here is our menu for you to pick from:\n");
    printf("VEG PIZZA:\n1. Farm Fresh Pizza\t\t Rs.320\n2. Quattro Formaggi Pizza\t Rs.320\n3. Al Funghi Pizza\t\t Rs.315\n4. Primavera Pizza\t\t Rs.315\n");
    printf("5. Spicy Paneer Pizza\t\t Rs.315\n6. Cheese and Corn Pizza\t Rs.300\n7. All Veg Pizza\t\t Rs.295\n8. Margherita Pizza\t\t Rs.275\n");
    printf("NON VEG PIZZA:\n9. Exotic Pizza\t\t\tRs.360\n");
    printf("10. Barbecue Chicken Pizza\tRs.335\n");
    printf("11. Grilled Chicken Pizza\tRs.335\n");
    printf("12. Keema Pizza\t\t\tRs.335\n");
    printf("13. Mustard Chicken Pizza\tRs.335\n");
    printf("14. Pizza E Hurricane\t\tRs.335\n");
    printf("15. Salami Delight Pizza\tRs.335\n");
    printf("16. Thai Chicken Pizza\t\tRs.335\n");
    printf("17. Bagna Cauda Pizza\t\tRs.330\n");
    printf("18. Smoked Chicken Pizza\tRs.315\n");
    printf("COLD COFFEE:\n19. Iced Espresso\t\tRs.250\n");
    printf("20. Coffee Addiction\t\tRs.180\n");
    printf("21. Dream Catcher\t\tRs.180\n");
    printf("22. Vegan Shake\t\t\tRs.180\n");
    printf("23. Caramel Crunchy Frappe\tRs.175\n");
    printf("24. Cafe Nostalgia\t\tRs.175\n");
    printf("25. Classic Irish\t\tRs.165\n");
    printf("COOLERS:\n26. Cumin Spice Cooler\t\tRs.165\n");
    printf("27. Black Virgin Mojito\t\tRs.165\n");
    printf("28. Cranberry Virgin Mojito\tRs.165\n");
    printf("29. Pineapple Virgin Mojito\tRs.165\n");
    printf("30. Cool Blue Cooler\t\tRs.150\n");
    printf("31. Cranberry Soda\t\tRs.150\n");
    printf("32. Lemon Peach Cooler\t\tRs.150\n");
    printf("33. Peach Iced Tea\t\tRs.125\n");
    printf("SHAKES:\n34. Blueberry Shake\t\tRs.170\n");
    printf("35. Brownie Nutty Shake\t\tRs.170\n");
    printf("36. Kesar Badaam Shake\t\tRs.170\n");
    printf("37. Mangoberry Shake\t\tRs.170\n");
    printf("38. Mango Kiwi Shake\t\tRs.170\n");
    printf("39. Red Velvet Shake\t\tRs.170\n");
    printf("40. Strawberry Shake\t\tRs.170\n");
    printf("41. Chocolate Shake\t\tRs.170\n");
    printf("HOT COFFEE:\n42. Cafe Caramel Hot Coffee\tRs.140\n");
    printf("43. Cafe Irish Hot Coffee\tRs.140\n");
    printf("44. Cafe Vanilla Hot Coffee\tRs.140\n");
    printf("45. Cappuccino Hot Coffee\tRs.125\n");
    printf("46. Irish Coffee\t\tRs.125\n");
    int i;
    for(i=1;i<47;i++)
        item[i].code=i;
    for(i=1;i<47;i++)
    {
        if(i==1)
        {
            strcpy(item[i].food,"Farm Fresh Pizza");
            item[i].price=320;
        }
        if(i==2)
        {
            strcpy(item[i].food,"Quattro Formaggi Pizza");
            item[i].price=320;
        }
        if(i==3)
        {
            strcpy(item[i].food,"Al Funghi Pizza");
            item[i].price=315;
        }
        if(i==4)
        {
            strcpy(item[i].food,"Primavera Pizza");
            item[i].price=315;
        }
        if(i==5)
        {
            strcpy(item[i].food,"Spicy Paneer Pizza");
            item[i].price=315;
        }
        if(i==6)
        {
            strcpy(item[i].food,"Cheese and Corn Pizza");
            item[i].price=300;
        }
        if(i==7)
        {
            strcpy(item[i].food,"All Veg Pizza");
            item[i].price=295;
        }
        if(i==8)
        {
            strcpy(item[i].food,"Margherita Pizza");
            item[i].price=275;
        }
        if(i==9)
        {
            strcpy(item[i].food,"Exotic Pizza");
            item[i].price=360;
        }
        if(i==10)
        {
            strcpy(item[i].food,"Barbecue Chicken Pizza");
            item[i].price=335;
        }
        if(i==11)
        {
            strcpy(item[i].food,"Grilled Chicken Pizza");
            item[i].price=335;
        }
        if(i==12)
        {
            strcpy(item[i].food,"Keema Pizza");
            item[i].price=335;
        }
        if(i==13)
        {
            strcpy(item[i].food,"Mustard Chicken Pizza");
            item[i].price=335;
        }
        if(i==14)
        {
            strcpy(item[i].food,"Pizza e Hurricane");
            item[i].price=335;
        }
        if(i==15)
        {
            strcpy(item[i].food,"Salami Delight Pizza");
            item[i].price=335;
        }
        if(i==16)
        {
            strcpy(item[i].food,"Thai Chicken Pizza");
            item[i].price=335;
        }
        if(i==17)
        {
            strcpy(item[i].food,"Bagna Cauda Pizza");
            item[i].price=330;
        }
        if(i==18)
        {
            strcpy(item[i].food,"Smoked Chicken Pizza");
            item[i].price=315;
        }
        if(i==19)
        {
            strcpy(item[i].food,"Iced Espresso");
            item[i].price=250;
        }
        if(i==20)
        {
            strcpy(item[i].food,"Coffee Addiction");
            item[i].price=180;
        }
        if(i==21)
        {
            strcpy(item[i].food,"Dream Catcher");
            item[i].price=180;
        }
        if(i==22)
        {
            strcpy(item[i].food,"Vegan Shake");
            item[i].price=180;
        }
        if(i==23)
        {
            strcpy(item[i].food,"Caramel Crunchy Frappe");
            item[i].price=175;
        }
        if(i==24)
        {
            strcpy(item[i].food,"Cafe Nostalgia");
            item[i].price=175;
        }
        if(i==25)
        {
            strcpy(item[i].food,"Classic Irish");
            item[i].price=165;
        }
        if(i==26)
        {
            strcpy(item[i].food,"Cumin Spice Cooler");
            item[i].price=165;
        }
        if(i==27)
        {
            strcpy(item[i].food,"Black Virgin Mojito");
            item[i].price=165;
        }
        if(i==28)
        {
            strcpy(item[i].food,"Cranberry Virgin Mojito");
            item[i].price=165;
        }
        if(i==29)
        {
            strcpy(item[i].food,"Pineapple Virgin Mojito");
            item[i].price=165;
        }
        if(i==30)
        {
            strcpy(item[i].food,"Cool Blue Cooler");
            item[i].price=150;
        }
        if(i==31)
        {
            strcpy(item[i].food,"Cranberry Soda");
            item[i].price=150;
        }
        if(i==32)
        {
            strcpy(item[i].food,"Lemon Peach Cooler");
            item[i].price=150;
        }
        if(i==33)
        {
            strcpy(item[i].food,"Peach Iced Tea");
            item[i].price=125;
        }
        if(i==34)
        {
            strcpy(item[i].food,"Blueberry Shake");
            item[i].price=170;
        }
        if(i==35)
        {
            strcpy(item[i].food,"Brownie Nutty Shake");
            item[i].price=170;
        }
        if(i==36)
        {
            strcpy(item[i].food,"Kesar Badaam Shake");
            item[i].price=170;
        }
        if(i==37)
        {
            strcpy(item[i].food,"Mangoberry Shake");
            item[i].price=170;
        }
        if(i==38)
        {
            strcpy(item[i].food,"Mango Kiwi Shake");
            item[i].price=170;
        }
        if(i==39)
        {
            strcpy(item[i].food,"Red Velvet Shake");
            item[i].price=170;
        }
        if(i==40)
        {
            strcpy(item[i].food,"Strawberry Shake");
            item[i].price=170;
        }
        if(i==41)
        {
            strcpy(item[i].food,"Chocolate Shake");
            item[i].price=170;
        }
        if(i==42)
        {
            strcpy(item[i].food,"Cafe Caramel Hot Coffee");
            item[i].price=140;
        }
        if(i==43)
        {
            strcpy(item[i].food,"Cafe Irish Hot Coffee");
            item[i].price=140;
        }
        if(i==44)
        {
            strcpy(item[i].food,"Cafe Vanilla Hot Coffee");
            item[i].price=140;
        }
        if(i==45)
        {
            strcpy(item[i].food,"Cappuccino Hot Coffee");
            item[i].price=125;
        }
        if(i==46)
        {
            strcpy(item[i].food,"Irish Coffee");
            item[i].price=125;
        }
    }
    printf("\n\n\nPress 1 to place an order.\n");
    printf("Press 0 if you didn't like anything.\n");
    printf("What would you like to do?");
    int n;
    scanf("%d",&n);
    switch(n)
    {
    case 0:
        printf("We're sorry to see that you didn't like anything.\nDo come back the next time and we'll try to surprise you with new delicacies!\n");
        break;
    case 1:
        printf("Enter the code for the menu item:");
        int a;
        scanf("%d",&a);
        for(i=1;i<47;i++)
        {
            if(a==i)
            {
                kitchen=fopen("kitchen.txt","w");
                fprintf(kitchen,"%s\n","ORDER");
                fprintf(kitchen,"%s\n",item[a].food);
                fclose(kitchen);
                P=P+item[a].price;
                bill=fopen("bill.txt","w");
                fprintf(bill,"%s\n","BILL");
                fprintf(bill,"%s %s %d\n",item[a].food,"Rs.",item[a].price);
                fclose(bill);
                printf("%s has been added to your order!\n\n",item[a].food);
                printf("Press 1 if you want to add another menu item to your order.\n");
                printf("Press 0 if your order is complete.\n");
                int b;
                printf("What would you like to do?\n");
                scanf("%d",&b);
                switch(b)
                {
                case 0:
                    printf("Your order has been placed, it will be served within a few minutes.\n");
                    printf("The amount due is Rs.%d.",P);
                    bill=fopen("bill.txt","a");
                    fprintf(bill,"%s %s %s %s %s %d","The","amount","due","is","Rs.",P);
                    fclose(bill);
                    exit(0);
                case 1:
                    printf("Enter the code for the menu item:");
                    int c;
                    scanf("%d",&c);
                    order(c);
                    break;
                }
            }
        }
        break;
    }
}
void order(int x)
{
    int j,n,d;
    for(j=1;j<47;j++)
    {
        if(x==j)
        {
            kitchen=fopen("kitchen.txt","a");
            fprintf(kitchen,"%s\n",item[x].food);
            fclose(kitchen);
            P=P+item[x].price;
            bill=fopen("bill.txt","a");
            fprintf(bill,"%s %s %d\n",item[x].food,"Rs.",item[x].price);
            fclose(bill);
            printf("%s has been added to your order!\n\n",item[x].food);
            printf("Press 1 if you want to add another menu item to your order.\n");
            printf("Press 0 if your order is complete.\n");
            printf("What would you like to do?\n");
            scanf("%d",&n);
            switch(n)
            {
                case 0:
                    printf("Your order has been placed, it will be served within a few minutes.\n");
                    printf("The amount due is Rs.%d.",P);
                    bill=fopen("bill.txt","a");
                    fprintf(bill,"%s %s %s %s %s %d","The","amount","due","is","Rs.",P);
                    fclose(bill);
                    exit(0);
                case 1:
                    printf("Enter the code for the menu item:");
                    scanf("%d",&d);
                    order(d);
                    break;
            }
        }
