# Elko automations

???+ question "How to setup Elko devices?"

    Most Elko devices use either Z-Wave or Zigbee protocols to connect to your Futurehome system. The specific setup process depends on which protocol your particular Elko device uses. 
    For detailed step-by-step instructions on adding Z-Wave and Zigbee devices to your Futurehome hub, please refer to the official Futurehome setup guides[^1].


???+ question "How to setup Tibber devices?"

    To set up automations using Tibber devices, you must first download and install the Tibber integration through the Futurehome app. Once the integration is installed and configured, 
    you can create automations based on Tibber data such as energy prices and consumption. Please see the official Futurehome integration guide for detailed setup instructions[^2].

## Consumption-based automation
Using real-time energy data from sensors like the Tibber Pulse, you can set up consumption-based automations that temporarily adjust heating device temperatures during high-consumption periods or peak pricing hours, 
then automatically restore the original temperature settings once the specified period ends.

???+ example "Example using Tibber pulse and Elko Smart Super Thermostat"

    In this example, we will use the Tibber Pulse and Elko Smart Super Thermostat to create an automation based on real-time consumption data.

    **Automation example 1** (Sensor data exceeds 5000 watt)
    
    ``` text
    # Given
    The user has a Tibber pulse connected to their Futurehome
    And they have an Elko Smart Super Thermostat configured
    And the current mode is "home"
    And the thermostat temperature is set to normal operation
    
    # When
    The Tibber pulse shows real-time power consumption exceeding 5000 watts
    
    # Then
    The Elko Smart Super Thermostat temperature should be set to 5° Celsius
    And after 20 minutes, the temperature should automatically return to 30° Celsius
    ```

## Sensor-based automation
N/A

## Spot price automation
N/A

## Time-based automation
Using a power regulator device, you can create time-based automations that automatically reduce power consumption during night hours when demand is typically lower.

???+ example "Example using Elko Smart Super Thermostat"

    In this example, we will use the Elko Smart Super Thermostat to create two automations based on the time of day..

    **Automation example 1** (During daytime)
    
    ``` text
    # Given
    The user has an Elko Smart Super Thermostat connected to their Futurehome
    And the current mode is set to "home"
    And it is currently before 07:00
    
    # When
    The time reaches 07:00 on any day
    
    # Then
    The Elko Smart Super Thermostat temperature should be set to 30° Celsius
    ```

    **Automation example 2** (During nighttime) 

    ``` text
    # Given
    The user has an Elko Smart Super Thermostat connected to their Futurehome
    And the current mode is set to "home"
    And it is currently before 00:00
    
    # When
    The time reaches 00:00 on any day
    
    # Then
    The Elko Smart Super Thermostat temperature should be set to 5° Celsius
    ```

[^1]:
[https://support.futurehome.no/hc/en-no/articles/360038993352-Inclusion-adding-a-device](https://support.futurehome.no/hc/en-no/articles/360038993352-Inclusion-adding-a-device)

[^2]:
[https://support.futurehome.no/hc/en-no/articles/360052072892-Tibber-Pulse](https://support.futurehome.no/hc/en-no/articles/360052072892-Tibber-Pulse)
