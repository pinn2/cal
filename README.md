#include<stdio.h>
main()
{
	float d,a,b,e,f,g;
	char p;
	int yes;
	printf("enter the number: ");
	scanf("%f",&a);
	printf("enter the second number: ");
	scanf("%f",&b);
	printf("which operation u want to do?:\n ");
	printf("enter for\n addition +\n substractin -\n multiplaction *\n divide /\n\n\n");
	scanf("%s",&p);
	
    switch (p)
	{
		case'+':
			d=a+b;
			printf("adiiton is:%f\n",d);
			break;
		case'-':
			e=a-b;
			printf("subtraction is:%f\n",e);
			break;	
		case'*':
		    f=a*b;
			printf("multiplaction is:%f\n",f);
			break;
		case'/':
		    if(b==0)
		    {
			printf("it gives 0..thats may be wrong\n");
			break;
		    }
			g=a/b;
			printf("divide is:%f\n",g);
			break;
		default:
		    printf("plzz enter any operation");
			break;			
	}
	printf("if u want to repeat plzz..enter 0 !\n\n");
	scanf("%d",yes);
	if(yes==0)
	{
		return main();
	}
	else
	{
	printf("thanks for using my caluculatr...!\n\n\n");
	return 0;
   }
}
	
