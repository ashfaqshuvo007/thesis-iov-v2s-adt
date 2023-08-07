# Harnessing Blockchain and Digital Twin for Security Risk Assessment in Internet of Vehicles

Digital Twins (DTs) are digital representations of their physical counterparts, used for testing, simulation, and prototyping before a physical component is manufactured. DT technology has been widely used in smart manufacturing for several years to improve every area of operations. Moreover, blockchain technology and DTs for industrial systems have gained traction among researchers in the last decade. On the other hand, with recent advancements in smart cities and Intelligent Transport Systems (ITS), the Internet of Vehicles (IoV) concept is becoming more prevalent. DT, which serves as a metric for creating virtual representations of real-world objects, offers enormous potential for enhancing the security and resilience of all parts of smart cities, including IoV, before being deployed in the real world. Very little research exists in the context of blockchain-based DTs as a security enhancer in IoV. In this thesis, we present a comprehensive systematic review of the existing literature where blockchain-based DTs have been suggested as extra security layers for industrial systems. Moreover, a novel blockchain-based security framework is proposed to handle security threats in IoV. Additionally, security threat modeling and risk management for IoV and how the proposed blockchain-based framework mitigates the risks are showcased. The proposed solution is evaluated using DT-based simulation for V2S communication as a use case using Microsoft Azure Digital Twin platform.

## Folder Structure:
- `./smart-contracts`: the solidity smart contracts for the components used in the proposed blockchain-based DT for Vehicle-to-Sensor communication scenario in the Internet of Vehicles.

- `./dt-models-dtdl`: the Digital Twins Definition Language (DTDL) ontology for the IoV components used to create twins for devices in the Azure Digital Twins (ADT) Explorer.

- `./data-simulators`: C# application written for each component like **Vehicle**, **Analyzer**, **Roadside Unit** which simulate device telemetry and connect to Azure cloud mimicing real entities to update their virtual counterparts.

- `./data-ingestors`: Azure function application written for each component like **Vehicle**, **Analyzer**, **Roadside Unit**. They subscribe to events attached with each device on Azure cloud. They feed off of the data sent by the simulators and update the digital twins in ADT explorer.