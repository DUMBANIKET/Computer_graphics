# Digital Differential Analyzer (DDA)

### in dda we use division which is not faster as compaired to breshanhan(idk the spelling)


```
#include<graphics.h>
#include<conio.h>
#include<dos.h>
#include<math.h>
#include<iostream.h>

 ```

### Include all the Above import statement 

basic Program
``` 
(import packages)

void main(){
int gm,gd=DETECT;
initgraph(&gd,&gm,"C://TC//BGI");
getch(); //<- important for displaying the output
closegraph();// <-dont use this you may sometimes not see the output

}

```


### Let's see the logic for DDA ALgorithm

```
void dda(int x1,int y1,int x2,int y2){
int dx=x2-x1;
int dy=y2-y1;
int steps=abs(dx)>abs(dy)?abs(dx):abs(dy);

float  xinc=dx/(float) steps;
float yinx=dy/(float)steps;

int x=x1;
int y=y1;

for (int i=0;i<=steps;i++){
putpixel(x,y,15);
x+=xinc;
y+=yinc;
delay(10);

}

}

```


### just call this function passing the following parameters
## dda(x1,y1,x2,y2);

# thanks


