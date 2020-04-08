#include "MSP.h"

int main()
	
{
	P1 ->SEL0 &= ~0x01;
	P1 ->SEL1 &= ~0x01;
	
	P1 ->DIR |= 0x01;
	
	P1 ->OUT &= ~0x01;
	
	P2 ->SEL0 &= ~0x07;
	P2 ->SEL1 &= ~0x07;
		
	P2 ->DIR |= 0x07;
	P2 ->OUT &= ~0x07;
	
	int i,j;
	int t = 300000;
	
	for(i=0; i<8; i++)
	{
		P2 -> OUT &= ~0x07;
		P2 -> OUT |= i;
		for(j=0; j<t; j++)
		{
			
		}
	}
	
	P2 ->OUT &= ~0x07;
	
	while(1)
	{
		P1 -> OUT ^= 0x01;
		P2 -> OUT ^= 0x04;
		for(j=0; j<t; j++)
		{
			
		}
	}
}
