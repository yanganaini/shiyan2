# shiyan2#include <stdio.h>
#include <stdlib.h>

struct Student
{
	char no[17];
	int mNo;
	int kNo;
};

int main()
{
	int N, M;
	int *arr = NULL;
	scanf("%d", &N);
	struct Student *stu = (struct Student *)malloc(N*sizeof(struct Student));
	for(int i=0; i<N; i++)
	{
		scanf("%s %d %d", (stu+i)->no, &(stu+i)->mNo, &(stu+i)->kNo);
	}
	scanf("%d", &M);
	arr = (int *)malloc(M*sizeof(int));
	for(int j=0; j<M; j++)
	{
		scanf("%d", (arr+j));
	}
	for(int k=0; k<M; k++)
	{
		for(int n=0; n<N; n++)
		{
			if((stu+n)->mNo == *(arr+k))
			{
				printf("%s %d\n", (stu+n)->no, (stu+n)->kNo);
			}
		}
		
	}
	return 0;
}


