# Model-U

The Model-U is a USBC breakout board designed by [Crane](https://github.com/Crane1195).  

It is specificly designed for use with DIY rectangle controllers  
If you need a wiring guide please check out the [Crane's Lab Discord](https://discord.com/invite/S3qgZWD)  

This repository contains the files necessary to order these boards from [JLCPCB](https://jlcpcb.com/).  
Please be aware that JLC does not have a great track record when it comes to SMT part assembly.  
Crane had several of these boards manufactured and had about a 5% failure rate so order at your own risk.  
I am not responsible if you recieve defective boards.  

If you plan to sell these I recommend testing them first.  
To do this you will need a USBC to USBC 3.1 gen 2 cable and a 24 pin USBC breakout board.  
Here are links to the breakout board and cable that I use.  
Breakout: https://amazon.com/dp/B07771CFFM or https://amazon.com/dp/B09L816S5W  
USB Cable: https://amazon.com/dp/B07THFJ1J5  

To test the boards you need a multimeter with a continuity testing mode.  
Start by connecting the Model U to the 24 pin breakout.  
Next put one lead of the meter on any pin of the model u and then drag the other lead of your meter across every pin on the 24 pin breakout.  
Use the chart below to determine which pins should have continuity.  
If you get continuity on a pin that should not have continuity, such as D+ on the MU getting coninuity on a GND pin, then the Model U is broken.  

The pins on the left are the Model U and the right is the 24 pin breakout.  

5V - VBUS (A4, A9, B4, B9)  
TX - RX1/2- (A10, B10)  
3V - RX1/2+ (A11, B11)  
Gnd - GND and Shield (if applicable) (A1, A12, B1, B12)  
D+ - D+ (Either A6 or B6 you will only get continuity on one)  
D- - D- (Either A7 or B7 you will only get continuity on one)  
RX - TX1/2- (A3, B3)  
D3V - TX1/2+ (A2, B2)  

The following is a short guide on the ordering proccess  

1. Download the files from this repository by clicking on "Code" and then on "Download Zip". Unzip the "Model-U-main.zip" but do not unzip the "Model-U_panel.zip" folders  
![](https://github.com/HTangl/Model-U/blob/main/JLC%20Ordering%20Guide%20Pics/Step%2000.png?raw=true)  

2. From the JLCPCB home page click on "Order now"  
![](https://github.com/HTangl/Model-U/blob/main/JLC%20Ordering%20Guide%20Pics/Step%2001.png?raw=true)  

3. On the next page click the "Add gerber file" button and select one of the "Model-U_panel.zip" files in the "Model-U JLC Files" folder. For this guide I'm using the 10 piece panel. Keep in mind JLC's minimum order quantity is 5 so since I'm using the 10 piece panel file I will end up with 50 individual breakout boards total.  
![](https://github.com/HTangl/Model-U/blob/main/JLC%20Ordering%20Guide%20Pics/Step%2002.png?raw=true)  

4. Change the delivery format to "Panel by Customer" and then input the amount of rows and columns needed, for the 10 piece panel it is 2 columns and 5 rows  
![](https://github.com/HTangl/Model-U/blob/main/JLC%20Ordering%20Guide%20Pics/Step%2003.png?raw=true)  

5. Scroll down and turn on the "SMT Assembly" slider, leave everything default and then click "Confirm"  
![](https://github.com/HTangl/Model-U/blob/main/JLC%20Ordering%20Guide%20Pics/Step%2004.png?raw=true)  

6. On the next page add the BOM and CPL files from the "Model-U JLC Files" folder. Then select the "Single Piece" button and then click "NEXT"  
![](https://github.com/HTangl/Model-U/blob/main/JLC%20Ordering%20Guide%20Pics/Step%2005.png?raw=true)  

7. On this page just leave everything default and click "NEXT"  
![](https://github.com/HTangl/Model-U/blob/main/JLC%20Ordering%20Guide%20Pics/Step%2006.png?raw=true)  

8. The final step will show you a preview of what the boards will look like. It is normal for the parts to be off center and only displayed on one board. JLC will place the parts correctly after you place the order. ALso note that if you are ordering less than 50 individual breakout boards you will still be charged for 100 resistors, this is normal and is just a JLC policy. For some small parts they have a minimum quantity. Lasty please do not use the price listed in this picture as a refrence, the price shown doesn't include tax or shipping and JLC does change their price from time to time. All you have to do now is click "SAVE TO CART" and then finish the checkout process  
![](https://github.com/HTangl/Model-U/blob/main/JLC%20Ordering%20Guide%20Pics/Step%2007.png?raw=true)
