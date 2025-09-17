# Futurehome automations

???+ question "How to setup Futurehome devices?"

    Most Futurehome devices use either Z-Wave or Zigbee wireless protocols to communicate with your Futurehome hub. The specific setup process depends on which protocol your device uses, 
    but both are designed for easy integration into your smart home system. For detailed step-by-step instructions on pairing and configuring Z-Wave and Zigbee devices with your Futurehome hub, please see the official device setup guide[^1].

## Consumption-based automation
Using data from real-time sensors like the Futurehome HAN, you can set up consumption-based automations to turn off devices during specific periods, then turn them back on afterward.

???+ example "Example using Futurehome HAN and Futurehome Smart Rele 16A"

    In this example, we will use the Futurehome HAN and Futurehome Smart Relay 16A to create an automation based on real-time consumption data.

    **Automation example 1** (Sensor data exceeds 8000 watt)
    
    ``` text
    # Given
    The user has a Futurehome HAN configured to their Futurehome
    And a Futurehome Smart Relay 16A is connected and currently turned on
    And the system mode is "home"
    
    # When
    The Futurehome HAN shows power consumption exceeding 8000 watts
    
    # Then
    The Futurehome Smart Relay should be turned off
    And after 10 minutes, the relay should automatically turn back on
    ```

## Sensor-based automation
N/A

## Spot price automation
N/A

## Time-based automation
N/A

[^1]:
[https://support.futurehome.no/hc/en-no/articles/360038993352-Inclusion-adding-a-device](https://support.futurehome.no/hc/en-no/articles/360038993352-Inclusion-adding-a-device)
