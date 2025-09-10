# Mill automation(s)

??? question "How to setup Mill-device(s)?"
    
    In order to set up automation for Mill, one must first download and install the Mill wifi integration on the futurehome app. Please see the official guide for more info[^1].

## Consumption-based automation
N/A

## Sensor-based automation
N/A

## Spot price automation
N/A

## Time-based automation
Using any of the panel(s) that Mill provides, one can set up time-based automation(s) that will cover the use based on when someone is in the house.

???+ example "Example using Mill Glass Smart WiFi Panel Heater"

    In this example we will be using the Mill Glass Smart WiFi Panel Heater Gen - 4 to create two automation(s) based on time of the day. 
    The same example can be applied on any other Mill product(s).

    **Automation example 1** (During daytime)
    
    ``` text
    # Given 
    We have a Mill Glass Panel Heater and want to set the temperature to 20° Celsius, activating it 
    at 07:00.

    # When
    Time is 07:00 all days and modus is home. 

    # Then
    Temperature of Mill Glass Panel Heater is set to 20° Celsius. 
    ```

    **Automation example 2** (During nighttime) 

    ``` text
    # Given 
    We have a Mill Glass Panel Heater and want to set the temperature to 5° Celsius, activating it 
    at 00:00.

    # When
    Time is 00:00 all days and modus is home. 

    # Then
    Temperature of Mill Glass Panel Heater is set to 5° Celsius. 
    ```

[^1]:
[https://support.futurehome.no/hc/en-no/articles/360045000592-Mill-wifi](https://support.futurehome.no/hc/en-no/articles/360045000592-Mill-wifi)


