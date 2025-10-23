# assignment1
for practice
#include<stdio.h>
#include<math.h>
int isAdams(int t){
    int r=0;
    while(t!=0){
        r = r*10 + t%10;
        t = t/10;
    }
    return r;
}

int main(){
    
    int x;
    printf("enter your number:");
    scanf("%d",&x);

    int square = pow(x,2);

    int f = isAdams(x);

    int q = pow(f,2);

    int i = isAdams(q);


    if(square==i){
        printf("it's an adams number");
    }else{
        printf("it's not an adams number");
    }

    return 0;

}
