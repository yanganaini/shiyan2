#include <stdio.h>
#include <string.h>
#include <windows.h>

int  main()
{
	char s1[99],s2[99],*p1,*p2;
	int n=0;

	printf("请输入字符串：");
	gets(s1);

	printf("请输入子串：");
	gets(s2);

	p1=s1;
	p2=s2;

	strlwr(s1);
	while(*p1!='\0')
	{
		if(*p1==*p2)
		{
				while(*p1==*p2&&*p2!='\0')
				{
					p1++;
					p2++;
				}
		}
		else
		{
				p1++;
		}
		if(*p2=='\0')
		{
				n++;
		}
			p2=s2;
	}
	
	printf("子串的个数为：%d\n",n);

    system("pause");
	return 0;
}# shiyan2
