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
