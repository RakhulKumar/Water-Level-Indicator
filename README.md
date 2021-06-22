# Water-Level-Indicator using 74HC147 and CD4511 (Simulated using Proteus 8 Professional)

## Algorithm

Most water level indicators for water tanks are based upon the number of LEDs that glow to indicate the corresponding level of water in the container. Here we present a digital version of the water level indicator. It uses a 7-segment display to show the water level in numeric form from 0 to 9.

The numeric water indicator circuit works off 5V regulated power supply. It is built around priority encoder IC 74HC147, BCD-to-7-segment decoder IC CD4511, 7-segment display LTS543 and a few discrete components.

When the water tank is empty, all the inputs of the priority encoder (74HC147) remain high. As a result, its output also remains high, making all the inputs of the BCD to 7-segment decoder (CD4511) low. The 7-segment display at this stage shows ‘0,’ which means the tank is empty. Similarly, when the water level reaches 1st position from bottom, the display shows ‘1,’ and when the water level reaches 8th position, the display shows ‘8.’ Finally, when the tank is full, all the inputs of 74HC147 become low and its output goes low to make all the inputs of CD4511 high. The display now shows ‘9,’ which means the tank is full.

