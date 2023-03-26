# Brehsnam Circle drwaing algo


```


#include<graphics.h>
#include<conio.h>
#include<dos.h>
#include<iostream.h>

void circle(int xc ,int yc,int x,int y){
    putpixel(xc+x,yc+y,RED);
     putpixel(xc-x,yc+y,RED);
      putpixel(xc+x,yc-y,RED);
       putpixel(xc-x,yc-y,RED);
        putpixel(xc+y,yc+x,RED);
         putpixel(xc-y,yc+x,RED);
          putpixel(xc+y,yc-x,RED);
           putpixel(xc-y,yc-x,RED);
}
void circleBres(int xc, int yc, int r)
{
    
    int x=0;
    int y=r;
    int d=3-2*r;
    
    circle(xc,yc,x,y);
    while(y>=x){
        x++;
        if(d>0){
            y--;
            d+=4*(x-y)+10;
            
        }
        else{
            
            d+=4*(x)+6;
            circle(xc,yc,x,y);
        }
    }
}
 


void main(){
    int gm,gd=DETECT;
    initgraph(&gd,&gm,"C://TC//bgi");
    circleBres(50 , 50, 30);
    
    getch();
}

```
