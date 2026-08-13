# motion-sensor

simple arduino motion sensor that sends messages to an LCD.

<img width="393" height="302" alt="IMG_3575" src="https://github.com/user-attachments/assets/6bb047fa-969a-41dc-8773-ce1c672ad6b3" />  

<h2>materials</h2>  

arduino uno r3, breadboard, usb 2.0 type-a to type-b cable, breadboard, grove pir motion sensor, jst connector cable, i2c lcd

<h2>instructions</h2>  

connect the arduino to your computer, download/update the arduino ide.

plug one end of the jst cable into pir motion sensor. cut the connector off the other end and strip the red, black, and white wires. plug red into the the positive rail of your breadboard, black into ground, and white into a digital pin. (ideally you solder it to a jumper wire, but i ran out of them)  

shove the lcd header pins into your breadboard. it takes some force, you're not going to break anything, so push like you've eaten breakfast today. next, use wires (ideally jumper wires, but again, i had none) to connect it to the arduino according to the below schematic. be slow and careful. mistakes here are a pain to rectify.  

<img width="1280" height="720" alt="diagram" src="https://github.com/user-attachments/assets/1876d073-8eb9-4c61-9163-4d08213b44d9" />  

note: doesn't really matter which digital pins you wire it to. also, a potentiometer is good to have, but it doesn't matter if you don't. can just leave V0 unwired, your lcd won't explode.  

youtube tutorial link: https://youtu.be/dpoBwmuE2QE?si=ueNhAPQwRMz0TZVe  

turn it on and copy-paste my code (pir_lcd_sketch.txt) into your arduino ide and press upload. make sure you change the stuff i commented in, if you wired to different digital pins (you probably did).  

if your lcd doesn't show text, the display might be too bright. by default, it's at max contrast. fix this by wiring V0 to ground with a strong resistor. if you have one, you can use a potentiometer, but it's not super necessary.  

last step, pray everything works.  

thanks for reading :)
