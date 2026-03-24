# 🚗 Teltonika Telemetry Adapter

A lightweight and extensible adapter for decoding telemetry data sent by Teltonika GPS tracking devices. This project parses raw AVL data packets and converts them into structured, human-readable formats for further processing, analytics, or integration into fleet management systems.

---

## 📌 Features

- Decode Teltonika AVL data packets (Codec8 / Codec8E / Codec16)
- Supports TCP/IP communication
- Extracts:
  - GPS data (latitude, longitude, altitude, speed, angle)
  - IO elements (digital/analog inputs, sensors)
  - Timestamp and priority
- Easily integrable with backend systems (FMS, IoT platforms, etc.)
- Lightweight and fast processing
- Extensible architecture for custom parsing

---

## 🏗️ Architecture Overview

### Components

- **TCP Listener** – Receives incoming data packets from devices  
- **Protocol Parser** – Handles Teltonika AVL decoding  
- **Data Decoder** – Converts binary to structured JSON  
- **Output Layer** – Sends data to DB, API, or message brokers  

---

## 📥 Supported Codecs

- Codec 8  
- Codec 8 Extended (Codec8E)  
- Codec 16 *(optional / extendable)*  

---

## 🚀 Getting Started

### Prerequisites

- Go 
- Basic understanding of TCP networking  
- Teltonika device configured to send data  

---
