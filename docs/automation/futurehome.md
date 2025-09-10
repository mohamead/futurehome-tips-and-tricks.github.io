# Futurehome automation(s)

??? question "How to setup Futurehome-device(s)?"

    Most Futurehome-device(s) uses Z-Wave or Zigbee. Please see the official guide for more info[^1].

??? question "How to setup Tibber-device(s)?"

    In order to set up automation for Tibber, one must first download and install the Tibber integration on the Futurehome app. Please see the official guide for more info[^2].

## Consumption-based automation
Using data from real time sensor(s) like Tibber pulse or Futurehome HAN, one can set up consumption-based automation to turn off
some device in given period, before turing it back on.

???+ example "Example using Tibber pulse and Futurehome Smart Rele 16A"

    In this example we will be using the Tibber pulse and Futurehome Smart Rele 16 to create a automation based on real time consumption data.

    **Automation example 1** (Sensor data exceeds 5000 watt)
    
    ``` text
    # Given 
    We have a Tibber pulse, and want to turn off Futurehome Smart Rele if Tibber pulse exceeds 
    5000 watt.

    # When
    Tibber pulse show(s) real time data over 5000 watt and modus is home, away, sleep or vacation.

    # Then
    Futurehome Smart Rele is turned off, and turned back again after 10 min. 
    ```

## Sensor-based automation
N/A

## Spot price automation
N/A

## Time-based automation
N/A

[^1]:
[https://support.futurehome.no/hc/en-no/articles/360038993352-Inclusion-adding-a-device](https://support.futurehome.no/hc/en-no/articles/360038993352-Inclusion-adding-a-device)

[^2]:
[https://support.futurehome.no/hc/en-no/articles/360052072892-Tibber-Pulse](https://support.futurehome.no/hc/en-no/articles/360052072892-Tibber-Pulse)