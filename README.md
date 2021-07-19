# EMA-Swing-Trader

This is my implementation of the RedK Slow_Smooth Average (RSS_WMA) to be used with OANDA.

The idea is to catch up as much information as possible with M1 - one minute, or S30 - 30 seconds candles, and smooth it out to be used for swing trading. To do so the raw price data gets filtered out with an EMA, which is passed to another EMA and forming the signal after reducing the noise with a third EMA. 

It is missing a better way to enter and exit the positions by using only a strong up or down gradient. I will try to build a bot that only opens up a new position, when the gradient is + or - 70 or 80 degree. 

Also a graphic with the EMA3 with the live data that works with every iteration needs to be added. 
Right now the graphic only gets plotted after a keyboard interuption. 
