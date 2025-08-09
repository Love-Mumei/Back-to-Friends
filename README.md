# Back-to-Friends
Arduino LCD Lyrics Display 🎵

This project displays timed lyrics on a 16x2 LCD using arduino and for simulation I used tinkercad and the Adafruit LiquidCrystal library.
Each word appears with a delay, making it appear synchronized with the song.

📋 Features
	* Displays lyrics line-by-line with timing delays.
	*	Uses a 16x2 LCD with I2C interface.
	*	Simple and customizable delays for each word.
	*	Loops the display continuously.

🛠 Requirements:
	*	Hardware
	*	Arduino Uno
	*	16x2 LCD with I2C backpack
	*	Jumper wire
	*	Arduino IDE
	*	Adafruit LiquidCrystal library

Install via Arduino IDE → Sketch → Include Library → Manage Libraries and search for Adafruit LiquidCrystal.

🔌 Wiring (For Arduino Uno):
	* GND > GND
	* Vcc > 5V
	* SDA > A4
	* SCL > A5

💻 Code Overview:
	*	lcd_1.begin(16,2); sets the LCD size to 16 columns and 2 row.
	*	lcd_.setBaclight(1); turns on the LCD backlight.
	*	delay(); adds the delay before the next word appears.
	*	lcd_1.clear(); clears the whole LCD.
	*	lcd_1.setCursor(0, 0); sets the starting point to column 0 and row 0.
	*	lcd_1.setCursor(0, 1); sets the starting point to column 0 and row 1 creating a new line.
