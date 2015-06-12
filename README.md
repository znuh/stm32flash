# stm32flash
This is a patched version of stm32flash

The original stm32flash is rather picky about communication with the target. It fails and aborts when there's still some old data left in the RX FIFO.
This version continously tries establishing a connection to the bootloader until it succeeds or the user aborts.
