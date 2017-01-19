# elevator-using-pic16f
https://drive.google.com/file/d/0B6XF6lUahohndlh2ZS02dUpUbkE/view?usp=sharing


void main()
{
adcon1 = 0x07;
trisa=0xFF;
trisc=0xFF;
trisd=0x00;
trisb=0x00;
portc=0x0F;
portb=0x00;
portd=0x00;
      while(1)
{
 if(RA0_bit==1)
{
   //at level ground
                              if(RC1_bit==1)
                              {
                              RD2_bit=1;
                              RD3_bit=0;  }
                               else if(RA1_bit==1&&RA2==1){
                               RD2_bit=0;
                               RD3_bit=0;}
                               delay_ms(500);
                               portb=dec2bcd(1);



                              if(rc2_bit==1){
                              RD2_bit=1;
                              RD3_bit=0;     }
                              if(RA3==1&&RA4==1){
                              RD2_bit=0;
                              RD3_bit=0;
                              portb=dec2bcd(2);
                              delay_ms(500);     }
                              if(rc3_bit==1){
                              RD2_bit=1;
                              RD3_bit=0;
                                            }
                              if(RA5==1){
                              RD2_bit=0;
                              RD3_bit=0;
                              portb=dec2bcd(3);
                              delay_ms(500);
                                          }
                              }

                if(RA2==0&&RA1==1){
                                    //at level one
                                   if(rc0_bit==1){
                                   RD3_bit=1;
                                   RD2_bit=0;
                                                  }
                                   if(RA0==1){
                                   RD3_bit=0;
                                   RD2_bit=0;
                                   portb=dec2bcd(0);
                                   delay_ms(500);
                                               }
                                   if(rc2_bit==1){
                                   RD2_bit=1;
                                   RD3_bit=0;
                                                 }
                                   if(RA3==1&&RA4==1) {
                                   RD2_bit=0;
                                   RD3_bit=0;
                                   portb=dec2bcd(2);
                                   delay_ms(500);
                                                       }
                                   if(rc3_bit==1){
                                   RD2_bit=1;
                                   RD3_bit=0;
                                                 }
                                   if(RA5==1) {
                                   RD2_bit=0;
                                   RD3_bit=0;
                                   portb=dec2bcd(3);
                                   delay_ms(500);
                                                       }

                                   }
                       if(RA4==1&&RA3==1){//at level two
                                        if(rc3_bit==1){
                                         RD2_bit=1;
                                         RD3_bit=0;
                                                       }
                                         if(RA5==1) {
                                         RD2_bit=0;
                                         RD3_bit=0;
                                         portb=dec2bcd(3);
                                         delay_ms(500);
                                                             }
                                         if(rc1_bit==1){
                                         RD3_bit=1;
                                         RD2_bit=0;
                                                       }
                                         if(RA2==1&&RA1==1) {
                                         RD3_bit=0;
                                         RD2_bit=0;
                                         portb=dec2bcd(1);
                                         delay_ms(500);
                                                             }
                                         if(rc0_bit==1){
                                       RD3_bit=1;
                                       RD2_bit=0;
                                                     }
                                       if(RA0==1) {
                                       RD3_bit=0;
                                       RD2_bit=0;
                                       portb=dec2bcd(0);
                                       delay_ms(500);
                                                           }
                                       }
                     if(RA5_bit==1){   //   at level three
                                   if(rc2_bit==1){
                                   RD3_bit=1;
                                    RD2_bit=0;
                                                 }
                                   if(RA3==1&&RA4==1) {
                                   RD3_bit=0;
                                   RD2_bit=1;
                                   portb=dec2bcd(2);
                                   delay_ms(500);
                                                       }
                                   if(rc1_bit==1){
                                   RD3_bit=1;
                                   RD2_bit=0;
                                                 }
                                   if(RA2==1&&RA1==1) {
                                   RD3_bit=0;
                                   RD2_bit=0;
                                   portb=dec2bcd(1);
                                   delay_ms(500);
                                                       }
                                   if(rc0_bit==1){
                                   RD3_bit=1;
                                   RD2_bit=0;
                                                 }
                                   if(RA0==1) {
                                   RD3_bit=0;
                                   RD2_bit=0;
                                   portb=dec2bcd(0);
                                   delay_ms(500);
                                                }

                             }


        }

}




