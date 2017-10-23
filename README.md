# HTS221_Driver

此项目的代码基于ST官方的 Platform-independent device driver for HTS221，主要修改如下：   
1. 增加了基于STM32Cube HAL的I2C驱动，使用STM32Cube HAL的工程可以直接调用此代码（hi2c1）。
2. 修正官方代码中的HTS221_DeActivate 和 HTS221_Activate的功能写反的问题。
3. 修正了HTS221_Get_Humidity函数中tmp数据类型的问题（应该是int32_t）。 

官方资源链接：   
http://www.st.com/en/mems-and-sensors/hts221.html

This project is based on ST official Platform-independent device driver for HTS221.   
Change List:  
1. Add I2C code for STM32Cube HAL, The projects use STM32Cube HAL can use this driver easily.
2. Fix HTS221_DeActivate and HTS221_Activate, acturally they are opposite in the official code.
3. fix the data type in HTS221_Get_Humidity, which should by int32_t.

The ST official resource for HTS221:  
http://www.st.com/en/mems-and-sensors/hts221.html
