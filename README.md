#include<stdio.h>

int CheckForPrime(int);
int i;

int main()
{
	int n1,PrimeNo;
	printf("Input any positive number:-\n");
	scanf("%d",&n1);
	i=n1/2;
	PrimeNo=CheckForPrime(n1);
	if(PrimeNo==1)
	{
		printf("The number %d is a prime number\n",n1);
	}
	else
	{
		printf("The number %d is not a prime number\n",n1);
	}
	return 0;
}

int CheckForPrime(int n1)
{
	if(i==1)
	{
		return 1;
	}
	else if(n1%i==0)
	{
		return 0;
	}
	else
	{
		i=i-1;
		CheckForPrime(n1);
	}
}
