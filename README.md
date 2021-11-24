# manue-card
// food management system
//By:purushottam
#include<stdio.h>

int a,m,b,c,stock=0;

void display()
		{
			
printf("=======================<<Menu>>=========================");
 printf("========================================================");

 printf("!    Code  !        Items               !   Price     !");
 printf("========================================================");

printf("!  Code 1: ! Price of Simple Burger is  !      Rs 20/-   !");
printf("!  Code 2: ! Price of non-veg Burger is !      Rs 30/-   !");
printf("!  Code 3: ! Price of coke is !   Rs 25/-   !");
printf("!  Code 4: ! Price of veg Pizza is!               Rs 45/-   !");
printf("!  Code 5: ! Price of non-veg pizza is  !      Rs 65/-   !");
printf("!=====================================================!");			                               
printf("!  Code 6:  Make the Bill.    		              !");			                                   
printf("!  Code 7:  Palace the New Order.                     !");
printf("=========================================================");

		}

void entry()
	{
			play:
printf("Enter the Product Code:");
	scanf("%d",&a);
	}

void product1()
	{
			c=20;
printf("<<veg-berger>>");

printf("Enter the quantity:");
scanf("%d",&b);
c=c*b;
stock=stock+c;
	}

void product2()
	{
printf("<<Non-veg berger>>");
printf("Enter the quantity:");
scanf("%d",&b);
c=30;
c=c*b;
stock=stock+c;
	}
void product3()
	{
printf("<<coke>>");
printf("Enter the quantity:");
scanf("%d",&b);
c=25;
c=c*b;
stock=stock+c;
	}

void product4()
	{
printf("<<Veg Pizza>>");

printf("Enter the quantity:");
scanf("%d",&b);
c=45;
c=c*b;
stock=stock+c;
	}
void product5()
	{
printf("<<Non-Veg Pizza>>");
printf("Enter the quantity:");
scanf("%d",&b);
c=65;
c=c*b;
stock=stock+c;
	}
void product6()
	{
printf("Net Bill is:%d",stock);

	}
void product7()
	{
printf("New program.");

printf("Net Bill is:%d",stock);

	}
 void fdisplay()
	{

printf("====================================================");
printf("Items             Rate           Qty           Cost");
printf("====================================================");

if(a==1)
		{
printf("veg-berger");
		}
if(a==2)
		{
printf("Non-veg berger");
		}

		if(a==3)
		{
printf("coke");
		}

if(a==4)
		{
printf("Veg Pizza");
		}

if(a==5)
		{
printf("Non-Veg Pizza");
		}
printf("====================================================");
printf("Net Bill is:  %d",stock);
 printf("====================================================");
	}

int main()
{
	int p;
	g:
printf("Enter the password:");\
	scanf("%d",&p);
	if(p==1)
	{
	 goto play;
	}
	if(p!=1)
	{
	 printf("<<Your Password is wrong entter again>>");
	 goto g;
	}
	play:
	display();
	entry();
				if(a==1)
				{
				product1();
				entry();
				}

				if(a==2)
				{
				product2();
				entry();
				}

				if(a==3)
				{
				product3();
				entry();
				}

				if(a==4)
				{
				product4();
				entry();
				}

				if(a==5)
				{
				product5();
				entry();
				}

				if(a==6)
				{
				product6();
				fdisplay();
				entry();
				}

				if(a==7)
				{
				product7();
				goto play;
				}

	return 0;
}
