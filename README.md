# STM32 MPU6050 library 
MPU6050 accelerometer & gyroscope library for STM32 microcontrollers with CubeMX generated HAL

## IMPORTANT

The library's dependency includes need to be included in your project's **main.h** file. Are they:

* The ...**_hal.h** header
* The ...**_hal_i2c.h** header (for I2C communication)

```C
/* For stm32f0xx */
#include <stm32f0xx_hal.h>
#include <stm32f0xx_hal_i2c.h>
   
/* For stm32f1xx */
#include <stm32f1xx_hal.h>
#include <stm32f1xx_hal_i2c.h>
    
/* For stm32f2xx */
#include <stm32f2xx_hal.h>
#include <stm32f2xx_hal_i2c.h>
    
/* For stm32f3xx */
#include <stm32f3xx_hal.h>
#include <stm32f3xx_hal_i2c.h>
    
/* For stm32f4xx */
#include <stm32f4xx_hal.h>
#include <stm32f4xx_hal_i2c.h>

```

## Documentation
The functions are declared and documented in the **mpu6050.h** file.

## I2C settings
The STM32 **I2C** communication channel must be previously configured. This library will not do this for you.

It is recommended to use **STM32CubeMX** to generate the code with the settings.

### Mode
The I2C communicator must be configured as **I2C mode**.

### I2C Speed Mode
**I2C Speed Mode** must be configured as **Fast Mode**

### I2C Clock Speed
**I2C Clock Speed** must be greater or equal to **400000Hz**

### Other settings
Keep other settings as default

**Wrong settings will cause errors.**

