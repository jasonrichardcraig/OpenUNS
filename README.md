![OpenUNS Logo](https://raw.githubusercontent.com/jasonrichardcraig/OpenUNS/main/openuns_logo.png)

**OpenUNS**  
*The Open Industrial Backbone*

A clean, geometric logo representing the Unified Namespace for SCADA, Measurement, GIS, Ticketing, and Field Data Capture.  
The interconnected nodes symbolize telemetry, hierarchy, and multi-tenant sharing across industrial domains.
# OpenUNS

**OpenUNS** is an open‑source Unified Namespace (UNS) for industrial automation, built on **OPC UA**, **SQL Server hierarchyid**, and **MQTT Sparkplug B**.  
It provides a free, standards‑driven backbone for SCADA, measurement, and IIoT systems — with paid support available for enterprises that need reliability, compliance, and integration expertise.

---

## 🚀 Mission
Industrial data is often siloed, fragmented, and locked behind proprietary systems.  
OpenUNS delivers a **single source of truth** for plant data by:

- Modeling assets and tags in a hierarchical **OPC UA namespace**.
- Persisting structure and values into **SQL Server with hierarchyid**.
- Distributing telemetry via **MQTT Sparkplug B** for scalable IoT/cloud integration.
- Enabling **multi‑tenant isolation and controlled sharing** between organizations.

---

## 🏗️ OpenUNS Architecture

OpenUNS is a full industrial platform built around a Unified Namespace (UNS).  
It integrates SCADA, measurement, schematics, P&ID visualization, GIS mapping, ticketing, forms, and field data capture into one open-source backbone.

---

### 🔌 Data Sources
- PLCs, RTUs, Flow Computers, Sensors
- Protocols: Modbus, DNP3, EtherNet/IP, ROC, TotalFlow
- External GIS data feeds (pipelines, wells, facilities)

---

### 🖧 Core UNS Layer
- **OPC UA Server Runtime**
  - Normalizes telemetry into a hierarchical namespace
  - Exposes tags, alarms, and metadata
- **SQL UNS (hierarchyid)**
  - Persists structure, values, and relationships
  - Supports multi-tenant isolation and controlled sharing
  - Stores schematics, tickets, GIS layers, and forms
- **MQTT Sparkplug B Broker**
  - Publishes UNS tags as lightweight telemetry
  - Enables scalable distribution to IoT/cloud consumers

---

### 📊 Application Modules
- **SCADA Dashboards**
  - Real-time monitoring, alarms, and control
- **Measurement**
  - Flow computer integration
  - Audit trails and regulatory reporting
- **Schematics & P&ID**
  - Hierarchical models mapped to diagrams
  - Interactive visualization of assets and processes
- **GIS**
  - Pipelines, wells, and facilities mapped geospatially
  - Integration of telemetry with spatial context
- **Ticketing**
  - Work orders, incidents, and maintenance tracking
  - Includes **Transloading Ticketing** for logistics and product movement
- **Forms**
  - Configurable templates for inspections, readings, and compliance
  - Offline-first field data capture
- **Field Data Capture**
  - Mobile/web forms for inspections and readings
  - Offline mode with sync to UNS

---

### 🌐 User Interfaces
- **Blazor Web App**
  - Multi-tenant dashboards
  - Role-based access and sharing controls
- **Mobile Clients**
  - Field data capture and forms
  - Offline-first design
- **GIS Viewer**
  - Map-based visualization of pipelines, wells, and facilities

---

### 👥 Tenants & Clients
- SCADA operators
- Measurement analysts
- Maintenance teams
- Field technicians
- GIS engineers
- Logistics coordinators (transloading)
- Enterprise systems (MES, ERP, Cloud Analytics)

---

### 📌 Visual Flow

Devices / Field Equipment ├── PLCs, RTUs, Flow Computers, Sensors └── Protocols: Modbus, DNP3, EtherNet/IP, ROC, TotalFlow
    ↓
OPC UA Server Runtime ├── Normalizes telemetry into hierarchical namespace └── Acts as SCADA core
    ↓
SQL UNS (hierarchyid) ├── Persists structure, values, relationships ├── Stores schematics, tickets, GIS layers, forms └── Supports multi-tenant isolation & sharing
    ↔
    MQTT Sparkplug B Broker ├── Publishes UNS tags as lightweight telemetry └── Enables scalable IoT / cloud distribution
    ↓
    Application Modules ├── SCADA Dashboards ├── Measurement ├── Schematics & P&ID ├── GIS (Pipelines, Wells, Facilities) ├── Ticketing (including Transloading) ├── Forms └── Field Data Capture
    ↓
    User Interfaces ├── Blazor Web App ├── Mobile Clients └── GIS Viewer
        ↓
        Tenants / Enterprise Systems ├── Operators, Analysts, Maintenance Teams, Field Technicians, GIS Engineers, Logistics Coordinators └── Integrations: MES, ERP, Cloud Analytics

