# HoppersChoppers45
Repository for Botball team
#include <kipr/botball.h>

int main()
{
    printf("Hello World\n");
    enable_servos();
    set_servo_position(0,0);
    msleep(500);
    return 0;
}
