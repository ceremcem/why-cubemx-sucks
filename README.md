# Why CubeMX Sucks

1. Uses high RAM (1.5GB)
2. Generates slow code (STM HAL is slow)
3. Does not let every bit of configuration to be done
4. Removes the user code (try creating a timer, editing its IRQ handler and then remove the timer)
5. Poor UX (You can't define a macro for the timer prescaler value unless you find the hidden checkbox on the right of the input and click "do not check")
6. It does the actual code organisation and it mixes the hardware configuration and the application logic in the same page, which you have no choice but to obey this choice.
7. When you can't perform a very specific configuration within the CubeMX (like a specific DMA configuration) half of your hardware configuration lies in CubeMX and the other lies within the code. You can't examine the whole configuration by the CubeMX in such situations.
8. STM HAL is buggy.
9. STM HAL is mostly undocumented.
