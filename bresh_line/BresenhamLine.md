# Bresenham's Line Algorithm
- it is way faster than the dda line drawing algorithm 
- it does calcuations in integer addition and subtraction
- it does not support anti~alising


### Decision Parameter's To Remember
```
p=2*dy-dx;

p+=2*dy-2*dx;

p+=2*dy;
```

## Algorithm Logic

```
 int dx,dy,p,x,y;
    dx=x2-x1;
    dy=y2-y1;
    x=x1;
    y=y1;
    p=2*dy-dx;
    
    while(x<x2){
        if (p>=0){
            putpixel(x,y,15);
            p+=2*dy-2*dy;
            y+=1;
            delay(40);
            
        }
        else{
            putpixel(x,y,15);
            p+=2*dy;
            delay(40);
            
       } x+=1;
    }
    
}
```

### that's all now you can use this funtion in the main Method :)

#thanks ^_^
