# OSlabWeek1
Trying!
#include &lt;stdio.h&gt;
#include &lt;string.h&gt;
#include &lt;stdlib.h&gt;
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
printf(&quot;Welcome to 4 seasons cafe!\nWe hope to serve you delicious and fresh food!\n&quot;);
printf(&quot;Here is our menu for you to pick from:\n&quot;);
printf(&quot;VEG PIZZA:\n1. Farm Fresh Pizza\t\t Rs.320\n2. Quattro Formaggi Pizza\t
Rs.320\n3. Al Funghi Pizza\t\t Rs.315\n4. Primavera Pizza\t\t Rs.315\n&quot;);
printf(&quot;5. Spicy Paneer Pizza\t\t Rs.315\n6. Cheese and Corn Pizza\t Rs.300\n7. All Veg
Pizza\t\t Rs.295\n8. Margherita Pizza\t\t Rs.275\n&quot;);
printf(&quot;NON VEG PIZZA:\n9. Exotic Pizza\t\t\tRs.360\n&quot;);
printf(&quot;10. Barbecue Chicken Pizza\tRs.335\n&quot;);
printf(&quot;11. Grilled Chicken Pizza\tRs.335\n&quot;);
printf(&quot;12. Keema Pizza\t\t\tRs.335\n&quot;);
printf(&quot;13. Mustard Chicken Pizza\tRs.335\n&quot;);
printf(&quot;14. Pizza E Hurricane\t\tRs.335\n&quot;);
printf(&quot;15. Salami Delight Pizza\tRs.335\n&quot;);
printf(&quot;16. Thai Chicken Pizza\t\tRs.335\n&quot;);
printf(&quot;17. Bagna Cauda Pizza\t\tRs.330\n&quot;);

printf(&quot;18. Smoked Chicken Pizza\tRs.315\n&quot;);
printf(&quot;COLD COFFEE:\n19. Iced Espresso\t\tRs.250\n&quot;);
printf(&quot;20. Coffee Addiction\t\tRs.180\n&quot;);
printf(&quot;21. Dream Catcher\t\tRs.180\n&quot;);
printf(&quot;22. Vegan Shake\t\t\tRs.180\n&quot;);
printf(&quot;23. Caramel Crunchy Frappe\tRs.175\n&quot;);
printf(&quot;24. Cafe Nostalgia\t\tRs.175\n&quot;);
printf(&quot;25. Classic Irish\t\tRs.165\n&quot;);
printf(&quot;COOLERS:\n26. Cumin Spice Cooler\t\tRs.165\n&quot;);
printf(&quot;27. Black Virgin Mojito\t\tRs.165\n&quot;);
printf(&quot;28. Cranberry Virgin Mojito\tRs.165\n&quot;);
printf(&quot;29. Pineapple Virgin Mojito\tRs.165\n&quot;);
printf(&quot;30. Cool Blue Cooler\t\tRs.150\n&quot;);
printf(&quot;31. Cranberry Soda\t\tRs.150\n&quot;);
printf(&quot;32. Lemon Peach Cooler\t\tRs.150\n&quot;);
printf(&quot;33. Peach Iced Tea\t\tRs.125\n&quot;);
printf(&quot;SHAKES:\n34. Blueberry Shake\t\tRs.170\n&quot;);
printf(&quot;35. Brownie Nutty Shake\t\tRs.170\n&quot;);
printf(&quot;36. Kesar Badaam Shake\t\tRs.170\n&quot;);
printf(&quot;37. Mangoberry Shake\t\tRs.170\n&quot;);
printf(&quot;38. Mango Kiwi Shake\t\tRs.170\n&quot;);
printf(&quot;39. Red Velvet Shake\t\tRs.170\n&quot;);
printf(&quot;40. Strawberry Shake\t\tRs.170\n&quot;);
printf(&quot;41. Chocolate Shake\t\tRs.170\n&quot;);
printf(&quot;HOT COFFEE:\n42. Cafe Caramel Hot Coffee\tRs.140\n&quot;);
printf(&quot;43. Cafe Irish Hot Coffee\tRs.140\n&quot;);
printf(&quot;44. Cafe Vanilla Hot Coffee\tRs.140\n&quot;);
printf(&quot;45. Cappuccino Hot Coffee\tRs.125\n&quot;);
printf(&quot;46. Irish Coffee\t\tRs.125\n&quot;);
int i;

for(i=1;i&lt;47;i++)
item[i].code=i;
for(i=1;i&lt;47;i++)
{
if(i==1)
{
strcpy(item[i].food,&quot;Farm Fresh Pizza&quot;);
item[i].price=320;
}
if(i==2)
{
strcpy(item[i].food,&quot;Quattro Formaggi Pizza&quot;);
item[i].price=320;
}
if(i==3)
{
strcpy(item[i].food,&quot;Al Funghi Pizza&quot;);
item[i].price=315;
}
if(i==4)
{
strcpy(item[i].food,&quot;Primavera Pizza&quot;);
item[i].price=315;
}
if(i==5)
{
strcpy(item[i].food,&quot;Spicy Paneer Pizza&quot;);
item[i].price=315;
}
if(i==6)

{
strcpy(item[i].food,&quot;Cheese and Corn Pizza&quot;);
item[i].price=300;
}
if(i==7)
{
strcpy(item[i].food,&quot;All Veg Pizza&quot;);
item[i].price=295;
}
if(i==8)
{
strcpy(item[i].food,&quot;Margherita Pizza&quot;);
item[i].price=275;
}
if(i==9)
{
strcpy(item[i].food,&quot;Exotic Pizza&quot;);
item[i].price=360;
}
if(i==10)
{
strcpy(item[i].food,&quot;Barbecue Chicken Pizza&quot;);
item[i].price=335;
}
if(i==11)
{
strcpy(item[i].food,&quot;Grilled Chicken Pizza&quot;);
item[i].price=335;
}
if(i==12)

{
strcpy(item[i].food,&quot;Keema Pizza&quot;);
item[i].price=335;
}
if(i==13)
{
strcpy(item[i].food,&quot;Mustard Chicken Pizza&quot;);
item[i].price=335;
}
if(i==14)
{
strcpy(item[i].food,&quot;Pizza e Hurricane&quot;);
item[i].price=335;
}
if(i==15)
{
strcpy(item[i].food,&quot;Salami Delight Pizza&quot;);
item[i].price=335;
}
if(i==16)
{
strcpy(item[i].food,&quot;Thai Chicken Pizza&quot;);
item[i].price=335;
}
if(i==17)
{
strcpy(item[i].food,&quot;Bagna Cauda Pizza&quot;);
item[i].price=330;
}
if(i==18)

{
strcpy(item[i].food,&quot;Smoked Chicken Pizza&quot;);
item[i].price=315;
}
if(i==19)
{
strcpy(item[i].food,&quot;Iced Espresso&quot;);
item[i].price=250;
}
if(i==20)
{
strcpy(item[i].food,&quot;Coffee Addiction&quot;);
item[i].price=180;
}
if(i==21)
{
strcpy(item[i].food,&quot;Dream Catcher&quot;);
item[i].price=180;
}
if(i==22)
{
strcpy(item[i].food,&quot;Vegan Shake&quot;);
item[i].price=180;
}
if(i==23)
{
strcpy(item[i].food,&quot;Caramel Crunchy Frappe&quot;);
item[i].price=175;
}
if(i==24)

{
strcpy(item[i].food,&quot;Cafe Nostalgia&quot;);
item[i].price=175;
}
if(i==25)
{
strcpy(item[i].food,&quot;Classic Irish&quot;);
item[i].price=165;
}
if(i==26)
{
strcpy(item[i].food,&quot;Cumin Spice Cooler&quot;);
item[i].price=165;
}
if(i==27)
{
strcpy(item[i].food,&quot;Black Virgin Mojito&quot;);
item[i].price=165;
}
if(i==28)
{
strcpy(item[i].food,&quot;Cranberry Virgin Mojito&quot;);
item[i].price=165;
}
if(i==29)
{
strcpy(item[i].food,&quot;Pineapple Virgin Mojito&quot;);
item[i].price=165;
}
if(i==30)

{
strcpy(item[i].food,&quot;Cool Blue Cooler&quot;);
item[i].price=150;
}
if(i==31)
{
strcpy(item[i].food,&quot;Cranberry Soda&quot;);
item[i].price=150;
}
if(i==32)
{
strcpy(item[i].food,&quot;Lemon Peach Cooler&quot;);
item[i].price=150;
}
if(i==33)
{
strcpy(item[i].food,&quot;Peach Iced Tea&quot;);
item[i].price=125;
}
if(i==34)
{
strcpy(item[i].food,&quot;Blueberry Shake&quot;);
item[i].price=170;
}
if(i==35)
{
strcpy(item[i].food,&quot;Brownie Nutty Shake&quot;);
item[i].price=170;
}
if(i==36)

{
strcpy(item[i].food,&quot;Kesar Badaam Shake&quot;);
item[i].price=170;
}
if(i==37)
{
strcpy(item[i].food,&quot;Mangoberry Shake&quot;);
item[i].price=170;
}
if(i==38)
{
strcpy(item[i].food,&quot;Mango Kiwi Shake&quot;);
item[i].price=170;
}
if(i==39)
{
strcpy(item[i].food,&quot;Red Velvet Shake&quot;);
item[i].price=170;
}
if(i==40)
{
strcpy(item[i].food,&quot;Strawberry Shake&quot;);
item[i].price=170;
}
if(i==41)
{
strcpy(item[i].food,&quot;Chocolate Shake&quot;);
item[i].price=170;
}
if(i==42)

{
strcpy(item[i].food,&quot;Cafe Caramel Hot Coffee&quot;);
item[i].price=140;
}
if(i==43)
{
strcpy(item[i].food,&quot;Cafe Irish Hot Coffee&quot;);
item[i].price=140;
}
if(i==44)
{
strcpy(item[i].food,&quot;Cafe Vanilla Hot Coffee&quot;);
item[i].price=140;
}
if(i==45)
{
strcpy(item[i].food,&quot;Cappuccino Hot Coffee&quot;);
item[i].price=125;
}
if(i==46)
{
strcpy(item[i].food,&quot;Irish Coffee&quot;);
item[i].price=125;
}
}
printf(&quot;\n\n\nPress 1 to place an order.\n&quot;);
printf(&quot;Press 0 if you didn&#39;t like anything.\n&quot;);
printf(&quot;What would you like to do?&quot;);
int n;
scanf(&quot;%d&quot;,&amp;n);

switch(n)
{
case 0:
printf(&quot;We&#39;re sorry to see that you didn&#39;t like anything.\nDo come back the next time and
we&#39;ll try to surprise you with new delicacies!\n&quot;);
break;
case 1:
printf(&quot;Enter the code for the menu item:&quot;);
int a;
scanf(&quot;%d&quot;,&amp;a);
for(i=1;i&lt;47;i++)
{
if(a==i)
{
kitchen=fopen(&quot;kitchen.txt&quot;,&quot;w&quot;);
fprintf(kitchen,&quot;%s\n&quot;,&quot;ORDER&quot;);
fprintf(kitchen,&quot;%s\n&quot;,item[a].food);
fclose(kitchen);
P=P+item[a].price;
bill=fopen(&quot;bill.txt&quot;,&quot;w&quot;);
fprintf(bill,&quot;%s\n&quot;,&quot;BILL&quot;);
fprintf(bill,&quot;%s %s %d\n&quot;,item[a].food,&quot;Rs.&quot;,item[a].price);
fclose(bill);
printf(&quot;%s has been added to your order!\n\n&quot;,item[a].food);
printf(&quot;Press 1 if you want to add another menu item to your order.\n&quot;);
printf(&quot;Press 0 if your order is complete.\n&quot;);
int b;
printf(&quot;What would you like to do?\n&quot;);
scanf(&quot;%d&quot;,&amp;b);
switch(b)
{

case 0:
printf(&quot;Your order has been placed, it will be served within a few minutes.\n&quot;);
printf(&quot;The amount due is Rs.%d.&quot;,P);
bill=fopen(&quot;bill.txt&quot;,&quot;a&quot;);
fprintf(bill,&quot;%s %s %s %s %s %d&quot;,&quot;The&quot;,&quot;amount&quot;,&quot;due&quot;,&quot;is&quot;,&quot;Rs.&quot;,P);
fclose(bill);
exit(0);
case 1:
printf(&quot;Enter the code for the menu item:&quot;);
int c;
scanf(&quot;%d&quot;,&amp;c);
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
for(j=1;j&lt;47;j++)
{
if(x==j)
{
kitchen=fopen(&quot;kitchen.txt&quot;,&quot;a&quot;);
fprintf(kitchen,&quot;%s\n&quot;,item[x].food);
fclose(kitchen);
P=P+item[x].price;

bill=fopen(&quot;bill.txt&quot;,&quot;a&quot;);
fprintf(bill,&quot;%s %s %d\n&quot;,item[x].food,&quot;Rs.&quot;,item[x].price);
fclose(bill);
printf(&quot;%s has been added to your order!\n\n&quot;,item[x].food);
printf(&quot;Press 1 if you want to add another menu item to your order.\n&quot;);
printf(&quot;Press 0 if your order is complete.\n&quot;);
printf(&quot;What would you like to do?\n&quot;);
scanf(&quot;%d&quot;,&amp;n);
switch(n)
{
case 0:
printf(&quot;Your order has been placed, it will be served within a few minutes.\n&quot;);
printf(&quot;The amount due is Rs.%d.&quot;,P);
bill=fopen(&quot;bill.txt&quot;,&quot;a&quot;);
fprintf(bill,&quot;%s %s %s %s %s %d&quot;,&quot;The&quot;,&quot;amount&quot;,&quot;due&quot;,&quot;is&quot;,&quot;Rs.&quot;,P);
fclose(bill);
exit(0);
case 1:
printf(&quot;Enter the code for the menu item:&quot;);
scanf(&quot;%d&quot;,&amp;d);
order(d);
break;
}
}
