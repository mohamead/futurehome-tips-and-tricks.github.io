# Futurehome automation

!!! Warning "Disclaimer"

    This page assumes familiarity with creating Futurehome automations. If you're new to automation setup, please consult the official Futurehome automation guide[^5]. The examples here focus on specific scenarios rather than basic automation creation steps.

The following page contains practical examples of automations you can configure in your Futurehome system. These real-world examples are organized by different device brands that are supported by Futurehome, 
making it easier to find relevant automation ideas for the specific products you own.

Each automation example is designed to demonstrate one or more of the four fundamental types of automations available in Futurehome:

| Type                            | Description                                                                                                                        |
|---------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
| 🔄 Consumption-based automation | A consumption-based automation is an action triggered by the power consumption of a device going above or below a given value[^1]. |
| 📈 Sensor-based automation      | A sensor-based automation is an automatic action triggered by a selected sensor reporting a specific state[^2].                    |
| 💰 Spot price automation        | A spot price automation is an action triggered based on the percentage above or below the daily average price from Nord Pool[^3].  |
| 🕐 Time-based automation        | A time-based automation is an action trigged based on a give time you choose[^4].                                                  |

These automation types form the building blocks for creating a truly smart and responsive home environment, allowing your devices to work together seamlessly based on various triggers and conditions.

!!! tip "Given-When-Then"

    The examples found under this page follow the Given-When-Then format used in documentation. The Given-When-Then format is a structured approach used in documentation, particularly within Behavior-Driven Development (BDD) and for writing acceptance criteria, to describe system behavior and scenarios clearly and consistently.
    This format provides a standardized way to describe automation scenarios that makes them easy to understand and replicate. Each automation example is broken down into three distinct components that clearly define the context, trigger, and expected outcome.
    
    **Given** establishes the initial context and preconditions for the automation. This section describes what devices are involved, their current state, and any necessary configuration settings that must be in place before the automation can function properly.
    
    **When** specifies the trigger event or condition that initiates the automation. This could be a time-based trigger, sensor reading, device state change, or user action that causes the Futurehome system to execute the automation sequence.
    
    **Then** describes the expected result or action that should occur when the trigger condition is met. This section outlines exactly what devices will respond, how they will change state, and what the end user should observe as the outcome of the automation.
    
    This structured approach ensures that each automation example is complete, unambiguous, and contains all the information needed to understand both the purpose and implementation of the automation. It also makes it easier to troubleshoot automations when they don't work as expected, since you can systematically check each component of the Given-When-Then scenario.

## Futurehome supported brands

The following list contains some of the brands currently supported by Futurehome for which automation examples are available on this site. Each brand section includes various types of automation scenarios to help you get the most out of your specific devices.

| Brand                       | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
|-----------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [ELKO](elko.md)             | ELKO is Norway's leading supplier of electrical equipment and has been producing sockets, light switches, and other electrical equipment for over 70 years. The company was founded in 1945 and has headquarters at Ryen in Oslo, Norway, with a production plant at Åmot in Modum.                                                                                                                                                                                                                           |
| [FUTUREHOME](futurehome.md) | FUTUREHOME is a Norwegian smart home technology company that was founded in Stavanger in 2013. The company developed a comprehensive smart home ecosystem that allowed users to control, automate, and monitor their homes remotely through a simple mobile app. Their system connected various smart devices throughout the home, with a particular focus on energy management solutions.                                                                                                                    |
| [MILL](mill.md)             | MILL is a Norwegian company that specializes in designing smart and beautiful heating and indoor climate products for modern homes. The company was founded in Norway in 1992 by Cato Bryn, initially focusing on the distribution of oil-filled radiators and other types of heaters. Over nearly two decades, from 1992 to 2009, Mill gained significant expertise in different types of heating solutions, which enabled them to establish relationships with major retailers across the Nordic countries. |

[^1]:
[https://support.futurehome.no/hc/en-no/articles/6438196230045-Consumption-based-automations](https://support.futurehome.no/hc/en-no/articles/6438196230045-Consumption-based-automations)

[^2]:
[https://support.futurehome.no/hc/en-no/articles/12040702126493-Sensor-based-automations](https://support.futurehome.no/hc/en-no/articles/12040702126493-Sensor-based-automations)

[^3]:
[https://support.futurehome.no/hc/en-no/articles/5067563218205-Spot-price-automations](https://support.futurehome.no/hc/en-no/articles/5067563218205-Spot-price-automations)

[^4]:
[https://support.futurehome.no/hc/en-no/articles/12040405232925-Time-based-automations](https://support.futurehome.no/hc/en-no/articles/12040405232925-Time-based-automations)

[^5]:
[https://support.futurehome.no/hc/en-no/articles/360039392291-Automations](https://support.futurehome.no/hc/en-no/articles/360039392291-Automations)
