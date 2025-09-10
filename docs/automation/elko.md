# Elko automation(s)

??? question "How to setup Elko-device(s)?"

    Most Elko-device(s) uses Z-Wave or Zigbee. Please see the official guide for more info[^1].

## Consumption-based automation
Using data from real time sensor(s) like Tibber pulse, one can set up consumption-based automation to adjust the temperature down for 
some device in given period, before adjusting it back up.

??? example "Example using Tibber pulse and Elko Smart Super Thermostat"

    In this example we will be using the Tibber pulse and Elko Smart Super Thermostat to create a automation based on real time consumption data.

    **Automation example 1** (Sensor data exceeds 5000 watt)
    
    ``` text
    # Given 
    We have a Tibber pulse, and want to set temperature to 5° Celsius on Elko Smart Super Thermostat 
    if Tibber pulse exceeds 5000 watt.

    # When
    Tibber pulse show(s) real time data over 5000 watt and modus is home, away, sleep or vacation.

    # Then
    Elko Smart Super Thermostat temperature is set to 5° Celsius, and after 20 min 
    it is set to 30° Celsius. 
    ```

## Sensor-based automation
N/A

## Spot price automation
N/A

## Time-based automation
Having a power regulator, one can set up time-based automation(s) that will force the unit to use less power during the night.

??? example "Example using Elko Smart Super Thermostat"

    In this example we will be using the Elko Smart Super Thermostat to create two automation(s) based on time of the day.

    **Automation example 1** (During daytime)
    
    ``` text
    # Given 
    We have a Elko Smart Super Thermostat and want to set the temperature to 30° Celsius, activating 
    it at 07:00.

    # When
    Time is 07:00 all days and modus is home. 

    # Then
    Temperature of Elko Smart Super Thermostat is set to 30° Celsius. 
    ```

    **Automation example 2** (During nighttime) 

    ``` text
    # Given 
    We have a Elko Smart Super Thermostat and want to set the temperature to 5° Celsius, activating 
    it at 00:00.

    # When
    Time is 00:00 all days and modus is home. 

    # Then
    Temperature of Elko Smart Super Thermostat is set to 5° Celsius. 
    ```

[^1]:
[https://support.futurehome.no/hc/en-no/articles/360038993352-Inclusion-adding-a-device](https://support.futurehome.no/hc/en-no/articles/360038993352-Inclusion-adding-a-device)
