# Example for oscilloscope CPU load

This app has a few tasks but settled on a simple approach to have a bit which is set when the CPU is busy and clear
when idle.   There are two key functions: Set_Busy() and Clear_Busy().   Each task must call Set_Busy() when it starts
(usually at top of its while(1) loop) and set Clear_Busy() just before calling vTaskDelay().   Tester can visualize busy state on oscilloscope. 
