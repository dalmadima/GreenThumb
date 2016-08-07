# GreenThumb

# Overview

+--------------+         +--------------+        +--------------+
|              |         |              |        |              |
|   Plant A    |         |   Plant B    |        |   Plant C    |
|              |         |              |        |              |
+--------+-----+         +-------+------+        +------+-------+
         |                       |                      |
         |                       |                      |
         |                       |                      |
         |                       +                      |
         |                     WiFi                     |
         |                       +                      |
         |                       |                      |
         |                       |                      |
         +----+ WiFi +--------+  |  +------+ WiFi +-----+
                              |  |  |
                          +---+--+--+---+
                          |             |
                          |             |
                          |Raspberry Pi |
                          |             |
                          |             |
                          |             |
                          |             |
                          +-------------+
                          |Touch Display|
                          +-------------+

Plant node:

- runs on ESP8266 with Arduino stack,
- connects soil moisture sensor, air hiumidity sensor, air temperature sensor, light sensor, (optional: CO2 sensor),
- brodcasts sensor data to central unit,
- receives and indicates with light actual plant comfort factor
- provides calibration interface,

Central unit node:

- maintains connectetions with plant nodes,
- logs all data from plant nodes,
- uses neural network for evaluating plant comfort factor,
- provides UI for all functions (eg. calibration, data overview, statistics, connecting new nodes),


# Task List

- neural network             - Margit
- UI interface	              - Stefan
- central unit architecture  - all
- plant node      		         - Dimitrie, Margitt
- watering system			         - Stefan
- architect					             - all
- light system				           - Kamil
- package				    	           - Kamil / all
- communication protocol     - all
