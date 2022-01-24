"`//将数据集中的地址转化为规则集中的地址 
#include<stdio.h>
#include<math.h>
int main()
{
	long long int n,a,b,c,d;
	scanf("%lld",&n);
	a=(n/16777216)%256;
	b=(n/65536)%256;
	c=(n/256)%256;
	d=n%256;
	printf("%lld.%lld.%lld.%lld",a,b,c,d);
	return 0;
}
//读取文件 
#include<stdio.h>
#include<stdlib.h>
int main()
{
FILE *file;
file = fopen("C:\\Users\\DEL\\Desktop\\Dev-Cpp\\file1.txt","r");
if(file==NULL)//如果未打开就提示读取错误
{
printf("read error");
} 
else
{
 printf("Yes");
 
}
char ch;
while((ch=fgetc(file))!=EOF)
{
	printf("%c",ch);
}
 fclose(file);//文件关闭函数
 } 
