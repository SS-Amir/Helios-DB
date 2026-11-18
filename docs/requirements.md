**🇬🇧 English |  [فارسی](requirements.fa.md)**

> **Note:** Color-coded formatting from the original `.docx` is preserved as emoji markers. Formatted PDF: [`source/Helios-db-RC.pdf`](source/Helios-db-RC.pdf) · Editable source: [`source/Helios-db-RC.docx`](source/Helios-db-RC.docx).

# Requirements Document

**Subject:** Database Requirements Document for Solar Power Plant Monitoring System

**Team Members:** E. Nima, P. Ali, S. Amir

Based on the requirements outlined below, please design the Entity-Relationship Diagram (ERD) and database structure for the Solar Power Plant Monitoring System so that unified management, monitoring, and performance analysis of the power plants are possible. The key points below summarize the client's requirements:

## 1. Power Plant and User Management

In this system, information for each 🔵 **User** is stored, including 🔵 National_ID (as a unique identifier), 🔵 Username, 🔵 Full_Name (consisting of 🔵 First_Name and 🔵 Last_Name), and 🔵 Phone_Numbers (where each person can have multiple phone numbers).

System users are categorized into three distinct roles (🟢 **Inheritance**): 🔵 **Admin** (which has the attribute 🔵 Seniority_Level), 🔵 **Expert** (which has the attribute 🔵 Field_of_Expertise), and 🔵 **Operator** (which has the attribute 🔵 Work_Shift).

Each 🔵 **Power_Plant** has a unique 🔵 Plant_ID, 🔵 Plant_Name, 🔵 Owner_Info, 🔵 Location (consisting of 🔵 Province, 🔵 City, and 🔵 Exact_Address), 🔵 Commissioning_Date, and 🔵 Total_Installed_Capacity (which is dynamically calculated from the sum of the capacities of the inverters located in that power plant).

For monitoring purposes, each power plant is assigned to one or more users, and each user can also be responsible for multiple power plants via 🟢 **Assignment**. During this assignment, recording the 🟢 Assignment_Start_Date and the 🟢 Granted_Access_Level for the user in that power plant is mandatory.

## 2. Power Plant Equipment (Inverter and Panel String)

One or more 🔵 **Inverter** units are deployed in each power plant via 🟢 **Deployment**, while each inverter belongs to only one specific power plant. Each inverter has a unique 🔵 Serial_Number, 🔵 Brand_Name, 🔵 Model, 🔵 Rated_Capacity, and 🔵 Connection_Type.

Furthermore, information for each 🔵 **Panel_String** is recorded in the system, including a unique 🔵 String_ID, 🔵 Panel_Count, 🔵 Panel_Type, and 🔵 Section_Capacity. Each inverter connects to one or more panel strings via 🟢 **Connection**, and each panel string is connected to only one inverter; when establishing this connection, the 🟢 Wiring_Method (series or parallel) and the 🟢 Input_Port_Number on the inverter must be recorded.

## 3. Performance Data and Register Maps

Due to the variety of inverter brands and models, an entity called 🔵 **Register_Map** is defined, which has a unique 🔵 Map_Code, 🔵 Protocol_Name, 🔵 Version, and 🔵 Communication_Parameters (which includes multiple different parameters). Each inverter follows only one register map based on its model via 🟢 **Follows**, whereas a single register map can be used by multiple inverters of the same model.

The system must store time-series 🟠 **Performance_Data** for each inverter. Since this data has no independent identity without an inverter, each performance data record is dependent on a specific inverter and is logged by it via 🟢 **Logs** (each inverter logs thousands of performance data records over time). Each record of this data is identified by a 🟠 Timestamp combined with the corresponding inverter's serial number, and includes the attributes 🟠 Voltage, 🟠 Generated_Power, 🟠 Generated_Energy, 🟠 Frequency, 🟠 Temperature, and 🟠 Operating_Status at that moment.

---

## Notation Legend

| Marker | Meaning |
|---|---|
| 🔵 **Bold** | Strong Entity |
| 🔵 Regular | Strong Entity Attribute |
| 🟠 **Bold** | Weak Entity |
| 🟠 Regular | Weak Entity Attribute |
| 🟢 **Bold** | Relationship |
| 🟢 Regular | Relationship Attribute |
