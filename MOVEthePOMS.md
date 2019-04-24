# HoppersChoppers45
Repository for Botball team
#include <kipr/botball.h>

int main()
{
    printf("Yes.\n");  //forward
    mav(0,-1500);
    mav(3,-4000);
    msleep(3200);
    
    mav(0,-100);
    mav(3,100);
    msleep(8767);
    
    mav(0,-1000);
    mav(3,-1000);
    msleep(1000);
    
    mav(0,1000);
    mav(3,1000);
    msleep(2000);
    return 0;
}
