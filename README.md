# 1D-pong

This is an ESP32 (at least that) version of the all well known warareg 1-D Pong game
also known as `one_d_pong`.

This is a linear pong game where the bat is a home area of about 7 pixels. Depending on
how deep you let the ball run into your home area, the faster it is repelled. If you 
fail to press the button in time you loose a point since the ball enters your home.
This version supports a boost button which sacrefies one pixel of your home area in 
favor of boosting your ball faster.

We discovered that using these Pins for I/O had quite some success

* GPIO19 = Right start/hit button (Y)
* GPIO18 = Right power-up button  (Y)
* GPIO33 = Left start/hit button  (X)
* GPIO23 = Left power-up button   (X)
* SOUND GPIO32  = Buzzer output (PB1/OC1A)

Some pins do not allow to configure Pull up resistors or work only as output. Don't use them.

We used Mouse devices which where re-soldered to use the 4 USB wires as 'short to GND' to work as controllers. 

