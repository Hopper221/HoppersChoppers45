# HoppersChoppers45
Repository for Botball team
#include <safty.h> //yes, it is spelled right.
#include <kipr/botball.h>
//|*************|
//| Dane Madsen |
//|             |
//|  2019 game  |
//|_____________|
int main()
{
    create_connect();
    //                                            DO NOT PICK UP ROBOT BY ARM... IT WILL DIE.
    printf("lets do this!\n");
    //getting out of the box...
    //and into the Fox
     wait_for_light(0);
    shut_down_in(118);
        create_drive_direct(500,-500);//get ready to pounce.
    msleep(300);
    create_stop();
    enable_servos();
                            // remember slowserv(port,starting position,destinaton,timen');
    slowserv(0,0,1385,100); //slowly bottom arm joint. MUST be the sameosite!!
   slowserv(1,2047,663,100);//ever so slowly second arm joint.
 set_servo_position(2,1024);//elbow shazam at top speed.
set_servo_position(3,1024); //hand, 90 will be straight out.Always slick ninja quick.
    msleep(5000);
    //ponder while Bill scootchies around a bit
    create_drive_direct(1000,1000);//scooch forward
    msleep(500);
    create_stop();
    create_drive_direct(-1000,1000);//SMITE THE POMS!!
     msleep(500);
     create_stop();
    create_drive_direct(900,1000);//scooch forwardish
    msleep(500);
    create_stop();
     create_drive_direct(-1000,1000);//RESMITE THE POMS!!
     msleep(500);
     create_stop();
    create_drive_direct(800,900);//rescooch forwardish
    msleep(500);
     create_drive_direct(-800,-200);//scooch backwardish-ish
    msleep(1000);
    create_stop();
    create_drive_direct(-1000,1000);//put the poms in the box.
    msleep(1000);
    create_stop();
    //Hi person looking at our code!
    set_servo_position(3,2047);//Open the claw.
    //Now for the "fun" part
      create_drive_direct(1000,-1000);//face your oponent
    msleep(1100);
    create_stop();
      create_drive_direct(1000,1000);//Move towards the adversary
    msleep(800);
    create_stop();
        set_servo_position(3,1000);// grab water?
    
    set_servo_position(2,2003);// lift!
     set_servo_position(0,0);
     set_servo_position(1,2047);
    
    return 0;
}
