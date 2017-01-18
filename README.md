# IRRemote for esp-open-rtos

Super simple IRRemote module for [esp-open-rtos](https://github.com/SuperHouse/esp-open-rtos).

Usage:

```c
// Enable GPIO pin and turn it off
gpio_enable(GPIO_IR_PIN, GPIO_OUTPUT);
gpio_write(GPIO_IR_PIN, 0);

// Set the GPIO pin
ir_set_pin(GPIO_IR_PIN);

// Send raw message
ir_send_raw(BUFFER, BUFFER_SIZE, 38);
```
