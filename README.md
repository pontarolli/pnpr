# Plug-and-Produce Architecture (PnPr)

Description of the steps of each process of PnPr architecture.

# Plug Process

Focused on commissioning and discovering assets.

## 1. Model
[aaspe](https://github.com/pontarolli/aaspe)

This repository outlines the standard naming conventions for files related to the Asset Administration Shell (AAS), applicable across different file formats. These conventions help in managing and automating processes within industrial systems, ensuring consistency and clarity in asset management.

## Standardization for Asset Administration Shell file names ( Package *.aasx)
Here we define the naming convention for `.aasx` packages, which encapsulate Asset Administration Shell data. This format is particularly used for exchanging data between systems in a secure and standardized manner. AAS type 1 interactions (Passive) for example via email or AAS type 2 interactions (Reactive) with standardized API (aasx-server).

- *Manufacturer_Description_Of_AAS_P&ID_Number_of_AAS.aasx* 
- BuschJost_Motor_Actuated_Proportional_Valve_82882009650_LV122_1.aasx
- Dancor_Centrifugal_Pump_CP4R_P1_1.aasx
- Dancor_Centrifugal_Pump_CP4R_P2_1.aasx
- Emerson_Pressure_Transmitter_2051_FIT116_1.aasx
- Emerson_Pressure_Transmitter_2051_LIT125_1.aasx
- Unesp_Service_Control_PID4_V001_1.aasx
- Wika_Electronic_Pressure_Switch_PSD4_PIT118_1.aasx
- Wika_Electronic_Pressure_Switch_PSD4_PIT129_1.aasx

## Standardization for Asset Administration Shell file names (JSON *.json)
This section outlines the naming conventions for `.json` files which are often used for AAS type 3 interactions (Proactive) for example exchanging messages between assets.

- *Manufacturer_Description_Of_AAS_P&ID_Number_of_AAS.json*
- BuschJost_Motor_Actuated_Proportional_Valve_82882009650_LV122_1.json
- Dancor_Centrifugal_Pump_CP4R_P1_1.json
- Dancor_Centrifugal_Pump_CP4R_P2_1.json
- Emerson_Pressure_Transmitter_2051_FIT116_1.json
- Emerson_Pressure_Transmitter_2051_LIT125_1.json
- Unesp_Service_Control_PID4_V001_1.json
- Wika_Electronic_Pressure_Switch_PSD4_PIT118_1.json
- Wika_Electronic_Pressure_Switch_PSD4_PIT129_1.json

## Standardization for Asset Administration Shell file names (OPC UA *.xml)
The `.xml` format is used in OPC UA environments to AAS type 3 interactions (Proactive) for example exchanging messages between assets.

- *Opc.Ua.Manufacturer_Description_Of_AAS_P&ID_Number_of_AAS.NodeSet2.xml*
- Opc.Ua.BuschJost_Motor_Actuated_Proportional_Valve_82882009650_LV122_1.NodeSet2.xml
- Opc.Ua.Dancor_Centrifugal_Pump_CP4R_P1_1.NodeSet2.xml
- Opc.Ua.Dancor_Centrifugal_Pump_CP4R_P2_1.NodeSet2.xml
- Opc.Ua.Emerson_Pressure_Transmitter_2051_FIT116_1.NodeSet2.xml
- Opc.Ua.Emerson_Pressure_Transmitter_2051_LIT125_1.NodeSet2.xml
- Opc.Ua.Unesp_Service_Control_PID4_1.NodeSet2.xml
- Opc.Ua.Wika_Electronic_Pressure_Switch_PSD4_PIT118_1.NodeSet2.xml
- Opc.Ua.Wika_Electronic_Pressure_Switch_PSD4_PIT129_1.NodeSet2.xml

## Standardization for AssetAdministrationShell idShort:
- *Manufacturer_Description_Of_AAS_P&ID_Number_of_AAS_Increasing_Number*
- BuschJost_Motor_Actuated_Proportional_Valve_82882009650_LV122_1
- Dancor_Centrifugal_Pump_CP4R_P1_1
- Dancor_Centrifugal_Pump_CP4R_P2_1
- Emerson_Pressure_Transmitter_2051_FIT116_1
- Emerson_Pressure_Transmitter_2051_LIT125_1
- Unesp_Service_Control_PID4_V001_1
- Wika_Electronic_Pressure_Switch_PSD4_PIT118_1
- Wika_Electronic_Pressure_Switch_PSD4_PIT129_1

## Standardization for Assets idShort:
- *Manufacturer_Description_Of_AAS_P&ID_Number_of_AAS*
- BuschJost_Motor_Actuated_Proportional_Valve_82882009650_LV122
- Dancor_Centrifugal_Pump_CP4R_P1
- Dancor_Centrifugal_Pump_CP4R_P2
- Emerson_Pressure_Transmitter_2051_FIT116
- Emerson_Pressure_Transmitter_2051_LIT125
- Unesp_Service_Control_PID4_V001
- Wika_Electronic_Pressure_Switch_PSD4_PIT118
- Wika_Electronic_Pressure_Switch_PSD4_PIT129




## 2. Aggregate
[aasx-server](https://github.com/pontarolli/aasx-server)

esse so mostra a padronizaçao anterior.

## 3. Servitize

## Standardization for Folders, GitHub, Microservices names and file names related with assets
For microservices and other related assets, the naming convention uses lowercase and hyphens to separate the elements, enhancing readability and manageability in software development. 

**Standarization for folders and GitHub repository names**
- *P&ID*
- lv122
- p1
- p2
- fit116
- lit125
- control
- pit118
- pit129

**Standarization for microservices names**
- *P&ID*  
- lv122
- p1
- p2
- fit116
- lit125
- control
- pit118
- pit129


**Standarization for microservices names**
- *P&ID.service.js*  
- lv122.service.js
- p1.service.js
- p2.service.js
- fit116.service.js
- lit125.service.js
- control.service.js
- pit118.service.js
- pit129.service.js

## 4. Install

## 5. Discover


# Produce Process

Focused on the composition of assets to create applications.

## 6. Communicate
## 7. Select
## 8. Analyze
## 9. Compose
## 10. Manage


