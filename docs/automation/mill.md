# Mill automations

???+ question "How to setup Mill-devices?"
    
    To set up automations for Mill devices, you must first download and install the Mill WiFi integration through the Futurehome app. Once the integration is installed and configured, you can create automations based on your Mill heating devices. 
    Please see the official integration guide for detailed setup instructions[^1].

## Consumption-based automation
N/A

## Sensor-based automation
N/A

## Spot price automation
N/A

## Time-based automation
Using any of the wifi panels that Mill provides, you can set up time-based automations that adjust heating based on occupancy patterns throughout the day. These smart automations can automatically lower temperatures during typical away hours, 
pre-heat rooms before you wake up or return from work, and maintain comfortable temperatures only when someone is actually home. This creates an efficient heating schedule that balances comfort with energy savings.

???+ example "Example using Mill Glass Smart WiFi Panel Heater"

    In this example, we will use the Mill Glass Smart WiFi Panel Heater to create two automations based on the time of day. The same example can be applied to any other Mill products.

    **Automation example 1** (During daytime)
    
    ``` text
    # Given 
    The user has an Mill Glass Smart WiFi Panel Heater connected to their Futurehome
    And the current mode is set to "home"
    And it is currently before 07:00

    # When
    The time reaches 07:00 on any day

    # Then
    Mill Glass Smart WiFi Panel Heater temperature should be set to 20° Celsius 
    ```

    **Automation example 2** (During nighttime) 

    ``` text
    # Given 
    The user has an Mill Glass Smart WiFi Panel Heater connected to their Futurehome
    And the current mode is set to "home"
    And it is currently before 00:00

    # When
    The time reaches 00:00 on any day

    # Then
    Mill Glass Smart WiFi Panel Heater temperature should be set to 15° Celsius 
    ```

[^1]:
[https://support.futurehome.no/hc/en-no/articles/360045000592-Mill-wifi](https://support.futurehome.no/hc/en-no/articles/360045000592-Mill-wifi)


