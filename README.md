# Plug-and-Produce Architecture (PnPr)

Description of the steps of each process of PnPr architecture.

# Plug Process

Focused on commissioning and discovering assets.

## 1. Model 

Standardization of the files of the Asset Administration Shell exported using the editor AAS Package Explorer. Here we define the naming convention for `.aasx` packages, which encapsulate Asset Administration Shell data. This format is particularly used for exchanging data between systems in a secure and standardized manner. AAS type 1 interactions (Passive) for example via email or AAS type 2 interactions (Reactive) with standardized API (aasx-server). The naming conventions for `.json` files which are often used for AAS type 3 interactions (Proactive) for example exchanging messages between assets. 
The `.xml` format is used in OPC UA environments to AAS type 3 interactions (Proactive) for example exchanging messages between assets.

### Naming Examples

| **Type**     | **AAS file**             | **AAS idShort**  | **Asset idShort** |
| ------------ | ------------------------ | ---------------- | ----------------- |
| **Template** | p&id-service.`extension` | aas-p&id-service | p&id-service      |
| **Sensors**  | fit116-daq.aasx          | aas-fit116-daq   | fit116-daq        |
|              | lit125-daq.json          | aas-lit125-daq   | lit125-daq        |
|              | pit118-daq.xml           | aas-pit118-daq   | pit118-daq        |
|              | pit129-daq.json          | aas-pit129-daq   | pit129-daq        |
| **Controls** | fic116-pid4.json         | aas-fic116-pid4  | fic116-pid4       |
|              | lic125-pid4.json         | aas-lic125-pid4  | lic125-pid4       |
|              | pic118-pid4.json         | aas-pic118-pid4  | pic118-pid4       |
|              | pic129-pid4.json         | aas-pic129-pid4  | pic129-pid4       |
| **Actuator** | lv122-daq.json           | aas-lv122-daq    | lv122-daq         |
|              | p1-daq.json              | aas-p1-daq       | p1-daq            |
|              | p2-daq.json              | aas-p2-daq       | p2-daq            |



## 2. Aggregate
[aasx-server](https://github.com/pontarolli/aasx-server)


## 3. Servitize

Standardization for GitHub, Microservices file and actions related with assets. For microservices and other related assets, the naming convention uses lowercase and hyphens to separate the elements, enhancing readability and manageability in software development. 

### Naming Examples

| **Type**     | **GitHub**   | **Microservice** | **Action**          |
| ------------ | ------------ | ---------------- | ------------------- |
| **Template** | p&id-service | p&id-service.js  | p&id-service.action |
| **Sensors**  | fit116-daq   | fit116-daq.js    | fit116-daq.aas      |
|              | lit125-daq   | lit125-daq.js    | lit125-daq.riin     |
|              | pit118-daq   | pit118-daq.js    | pit118-daq.ruout    |
|              | pit129-daq   | pit129-daq.js    | pit129-daq.wuout    |
| **Controls** | fic116-pid4  | fic116-pid4.js   | fic116-pid4.control |
|              | lic125-pid4  | lic125-pid4.js   | lic125-pid4.control |
|              | pic118-pid4  | pic118-pid4.js   | pic118-pid4.aas     |
|              | pic129-pid4  | pic129-pid4.js   | pic129-pid4.aas     |
| **Actuator** | lv122-daq    | lv122-daq.js     | lv122-daq.aas       |
|              | p1-daq       | p1-daq.js        | p1-daq.riin         |
|              | p2-daq       | p2-daq.js        | p2-daq.wuout        |




## 4. Install

Standarization for docker images names and containers

### Naming Examples

| **Type**     | **DockerHub images**                       | **Container name**    |
| ------------ | ------------------------------------------ | --------------------- |
| **Template** | gasiepgody/moleculer:p&id-service-v1.0.0   | p&id-service-v1.0.0   |
| **Sensors**  | gasiepgody/moleculer:fit116-daq-v1.0.0     | fit116-daq-v1.0.0     |
|              | gasiepgody/moleculer:lit125-daq-v1.0.0     | lit125-daq-v1.0.0     |
|              | gasiepgody/moleculer:pit118-daq-v1.0.0     | pit118-daq-v1.0.0     |
|              | gasiepgody/moleculer:pit129-daq-v1.0.0     | pit129-daq-v1.0.0     |
| **Controls** | gasiepgody/moleculer:fic116-control-v1.0.0 | fic116-control-v1.0.0 |
|              | gasiepgody/moleculer:lic125-control-v1.0.0 | lic125-control-v1.0.0 |
|              | gasiepgody/moleculer:pic118-control-v1.0.0 | pic118-control-v1.0.0 |
|              | gasiepgody/moleculer:pic129-control-v1.0.0 | pic129-control-v1.0.0 |
| **Actuator** | gasiepgody/moleculer:lv122-daq-v1.0.0      | lv122-daq-v1.0.0      |
|              | gasiepgody/moleculer:p1-daq-v1.0.0         | p1-daq-v1.0.0         |
|              | gasiepgody/moleculer:p2-daq-v1.0.0         | p2-daq-v1.0.0         |

## 5. Discover

# Produce Process

Focused on the composition of assets to create applications.

## 6. Communicate
## 7. Select
## 8. Analyze
## 9. Compose
## 10. Manage


