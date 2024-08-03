# Plug-and-Produce Architecture (PnPr)

Description of the steps of each process of PnPr architecture.

# Plug Process

Focused on commissioning and discovering assets.

## 1. Model 

Standardization of the files of the Asset Administration Shell exported using the editor AAS Package Explorer. Here we define the naming convention for `.aasx` packages, which encapsulate Asset Administration Shell data. This format is particularly used for exchanging data between systems in a secure and standardized manner. AAS type 1 interactions (Passive) for example via email or AAS type 2 interactions (Reactive) with standardized API (aasx-server). The naming conventions for `.json` files which are often used for AAS type 3 interactions (Proactive) for example exchanging messages between assets. 
The `.xml` format is used in OPC UA environments to AAS type 3 interactions (Proactive) for example exchanging messages between assets.

### Asset Administration Shell (AAS) - Standardization of names
Message from AAS Package Explorer: The idShort shall only feature letters, digits, underscore ('_'); starting mandatory with a letter.

| **Type**     | ** AAS File**            | **AAS and Asset idShort** |
| ------------ | ------------------------ | ------------------------- |
| **Template** | p&id_service.`extension` | p&id_service              |
| **Sensors**  | fit116_daq.aasx          | fit116_daq                |
|              | lit125_daq.json          | lit125_daq                |
|              | pit118_daq.xml           | pit118_daq                |
|              | pit129_daq.json          | pit129_daq                |
| **Controls** | fic116_pid4.json         | fic116_pid4               |
|              | lic125_pid4.json         | lic125_pid4               |
|              | pic118_pid4.json         | pic118_pid4               |
|              | pic129_pid4.json         | pic129_pid4               |
| **Actuator** | lv122_daq.json           | lv122_daq                 |
|              | p1_daq.json              | p1_daq                    |
|              | p2_daq.json              | p2_daq                    |




## 2. Aggregate
[aasx-server](https://github.com/pontarolli/aasx-server)


## 3. Servitize

### Microservices (μS) - Standardization of names


| **Type**     | **μS Name**  | **μS Action**       |
| ------------ | ------------ | ------------------- |
| **Template** | p&id_service | p&id_service.action |
| **Sensors**  | fit116_daq   | fit116_daq.aas      |
|              | lit125_daq   | lit125_daq.aas      |
|              | pit118_daq   | pit118_daq.aas      |
|              | pit129_daq   | pit129_daq.aas      |
| **Controls** | fic116_pid4  | fic116_pid4.control |
|              | lic125_pid4  | lic125_pid4.aas     |
|              | pic118_pid4  | pic118_pid4.aas     |
|              | pic129_pid4  | pic129_pid4.aas     |
| **Actuator** | lv122_daq    | lv122_daq.aas       |
|              | p1_daq       | p1_daq.aas          |
|              | p2_daq       | p2_daq.aas          |

Services have many more actions than these, and should be consulted individually.

## 4. Install


### Docker - Standardization of names

| **Type**     | **DockerHub images**                     | **Container name**  |
| ------------ | ---------------------------------------- | ------------------- |
| **Template** | gasiepgody/moleculer:p&id_service_v1.0.0 | p&id_service        |
| **Sensors**  | gasiepgody/moleculer:fit116_daq_v1.0.0   | fit116_daq          |
|              | gasiepgody/moleculer:lit125_daq_v1.0.0   | lit125_daq          |
|              | gasiepgody/moleculer:pit118_daq_v1.0.0   | pit118_daq          |
|              | gasiepgody/moleculer:pit129_daq_v1.0.0   | pit129_daq          |
| **Controls** | gasiepgody/moleculer:fic116_pid4_v2.0.0  | fic116_pid4         |
|              | gasiepgody/moleculer:lic125_pid4_v2.0.0  | lic125_pid4         |
|              | gasiepgody/moleculer:pic118_pid4_v2.0.0  | pic118_pid4         |
|              | gasiepgody/moleculer:pic129_pid4_v2.0.0  | pic129_pid4         |
| **Actuator** | gasiepgody/moleculer:lv122_daq_v1.0.0    | lv122_daq           |
|              | gasiepgody/moleculer:p1_daq_v1.0.0       | p1_daq              |
|              | gasiepgody/moleculer:p2_daq_v1.0.0       | p2_daq              |

## 5. Discover

# Produce Process

Focused on the composition of assets to create applications.

## 6. Communicate
## 7. Select
## 8. Analyze
## 9. Compose
## 10. Manage


