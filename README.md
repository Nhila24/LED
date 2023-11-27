First of all open STM32cubeIDE and chose Nucleo F446RE board. After choosing the board In STM32CubeIDE, from the Project Explorer tab, open the main.c file, in Src folder and add the adequate functions for the LED blinking, using HAL functions
Add the code given under the infinite loop.

	  HAL_GPIO_WritePin(GPIOA, GPIO_PIN_5, 1);
	  HAL_Delay(1000);
	  HAL_GPIO_WritePin(GPIOA, GPIO_PIN_5, 0);
	  HAL_Delay(1000);
After adding the code connect the F446RE board to  PC which will automatically update the board and run the program which will upload the code to the board.After restarting board we can see a blinking green LED on the board.
The delay can be adjusted to the timing we wanted it to blink.As per the code given above the LED will blink every second(1000ms).
![image](https://github.com/Nhila24/LED/assets/150771903/ff6705eb-02eb-4246-bcb2-2f02acdfe5d5)


Link to video:https://drive.google.com/file/d/1q5esRHA0ay1_Q4BqHPrXVY7x8BDx-f17/view?usp=drive_link
