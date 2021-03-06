# How to set up CCS compiler for Proteus ?
## You can run simulations either by using CCS compiler in Proteus (firmware project) or you have to run ELF file by taking them from CCS( also modifying CCS compiler in the process) - (non-firmware project)

 I don't have enough time to give all instructions step by step, but you can set up CCS compiler and then clone my repository and after figuring out by yourself more can run simulations in proteus. Also for running Hardware UART programs, you have to modify the program to Software UART and compile and run them through HEX files. because the Hardware UART does not give out any signal. Also the bounce debounce such things don't apply here, So getting a lunchbox in hand is the best way.
 
 ### This is a software UART (modified program from original ): 
 ![Exp41_LunchBox_Introduction_to_Embedded_C-INO.png](https://github.com/Subhankar2000/MSP430G2553-Proteus-v8.9-Simulation/blob/master/blob/Exp41_LunchBox_Introduction_to_Embedded_C-INO.png)
 
 ### Another Hello world ( software UART -  (modified program from original ) ) :
 ![Exp01_LunchBox_UART_Template-INO.png](https://github.com/Subhankar2000/MSP430G2553-Proteus-v8.9-Simulation/blob/master/blob/Exp01_LunchBox_UART_Template-INO.png)
  
 ### This is as per lecture video and using Embedded C code : 
 ![Exp05_LunchBox_DebouncingTheSwitch.png](https://github.com/Subhankar2000/MSP430G2553-Proteus-v8.9-Simulation/blob/master/blob/Exp05_LunchBox_DebouncingTheSwitch.png)
 
#### For using the Repository and my project files, you need to have CCS installed and integrated into Proteus, then you can use my files, but the UART ones need more guide to run( currently I am not able to write that much documentation )

## A way to integrate CCS compiler with Proteus : 
(a not so detailed way of explanation)

+ Step 1 : find the CCS installation directory , go to it :

![1.png](https://github.com/Subhankar2000/MSP430G2553-Proteus-v8.9-Simulation/blob/master/blob/1.png)

+ Step 2 : open proteus and select new project, do next next and come to this window :

![2.png](https://github.com/Subhankar2000/MSP430G2553-Proteus-v8.9-Simulation/blob/master/blob/2.png)

+ Step 3 : then select compilers and then search for Code Composer for MSP430 : and enter like this with your proper path and drive letter : 

![3.png](https://github.com/Subhankar2000/MSP430G2553-Proteus-v8.9-Simulation/blob/master/blob/3.png)

if you have installed typically in c drive and version as per NPTEL lecture, then your path may be like this : C:\ti\ccs930\ccs\tools\compiler\ti-cgt-msp430_18.12.4.LTS

Then clone my repository and open the Proteus project files and work with them, for UART, I will have to give detail explanation, but other than that any program having non-serial functionality should work, and exceptions will always be there for not working, you will have to figure it out.

Hope this all helps and any one else trying out on proteus due to lack of hardware do contribute.

Thank You

## Week wise distribution of Simulations
+ Week 7
	* Exp00_LunchBox_Template
	* Exp00_LunchBox_Template-ELF
	* Exp01_LunchBox_UART_Template-INO
	* Exp02_LunchBox_HelloLED
	* Exp03_LunchBox_HelloBlink
	* Exp04_LunchBox_HelloSwitch
	* Exp05_LunchBox_DebouncingTheSwitch
	* Exp06_LunchBox_HelloSwitch_PullDown
	* Exp07_LunchBox_HelloSwitch_PullUp
	* Exp41_LunchBox_Introduction_to_Embedded_C-INO
+ Week 8
	* Exp08_LunchBox_HelloClock
	* Exp09_LunchBox_HelloResetSource-Not working (unknown fault)
	* Exp10_LunchBox_HelloInterrupt
	* Exp11_LunchBox_HelloInterrupt_Rising
	* Exp12_LunchBox_HelloInterrupt_Falling
	* Exp12_LunchBox_HelloInterrupt_Falling-Exercise
	* Exp12_LunchBox_HelloInterrupt-Rising_Falling-Exercise
+ Week 9
	* Exp13_LunchBox_HelloSSD-modified P1p2
	* Exp14_LunchBox_HelloLPM
	* Exp15_LunchBox_HelloLCD-P2 instead of P1
	* Exp16_LunchBox_HelloLCDWithCustomCharacter-P2 instead of P1
	* Exp17_LunchBox_HelloTimer
+ Week 10
	* Exp18_LunchBox_HelloSoftwarePWM_Large_Delay
	* Exp18_LunchBox_HelloSoftwarePWM_Small_Delay
	* Exp19_LunchBox_HelloHardwarePWM_8Bit-Not working (unknown fault)
	* Exp20_LunchBox_HelloHardwarePWM_16Bit-Not working (unknown fault)
	* Exp21_LunchBox_HelloADC-Not working (unknown fault)
	* Exp22_LunchBox_HelloADC_LCD-Not working (unknown fault)
	* Exp23_LunchBox_HelloADC_Internal_Temperature_Sensor
	* Exp24_LunchBox_HelloLFSR_8Bit-P2 instead of P1
	* Exp25_LunchBox_HelloLFSR_32Bit
	* Exp26_LunchBox_HelloDAC_4Bit-P2 instead of P1
	* Exp26_LunchBox_HelloDAC_8Bit-P2 instead of P1
	* Exp27_LunchBox_Lemon_Battery_LED_Blink
+ Week 11
	* Exp28_LunchBox_HelloSerial
	* Exp29_LunchBox_HelloPeriod
	* Exp30_LunchBox_HelloFrequency
	* ...
+ Week 12 
	* ...