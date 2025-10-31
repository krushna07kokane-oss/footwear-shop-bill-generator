# footwear-shop-bill-generator

#include <stdio.h>
int main (){
    printf("----------------------  Welcome to the shop------------------------\n");

    int quantity,GST,The_final_price;
    int price,Total,discount;
    char customer_name[30];
    char product_type[20];

    printf("Name of customer:");
    scanf("%s",&customer_name);

   printf("Name of the product:");
   scanf("%s",&product_type);

   printf("The price of that product:");
   scanf("%d",&price);

   printf("quantity of product:");
   scanf("%d",&quantity);

   Total=price*quantity;
   printf("The total price is:%d\n",Total);

   //The discount on each product is 10%
  discount=Total*0.1;
   printf(" discount is:%d\n",discount);
     //The GST on the product by the goverment is 5%
     GST=Total*0.05;
     printf("The GST is:%d\n",GST);
     printf("\n----------------------------------------------------\n");

     The_final_price=Total+GST-discount;
     printf("The final prize is:%d\n",The_final_price);
     printf("\n-----------------Thank you visit again---------------\n");
    

return 0;
}
