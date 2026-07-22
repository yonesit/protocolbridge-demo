# Protocolbridge

> IIoT-Middleware zur Verbindung von Modbus, OPC UA und MQTT über eine gemeinsame REST API und ein Echtzeit-Dashboard.

## Überblick

**Protocolbridge** ist ein von Yones Alizai entwickeltes Softwareprojekt aus den Bereichen IIoT, Systemintegration und industrielle Kommunikation.

Das System verarbeitet Daten aus unterschiedlichen Kommunikationsprotokollen, normalisiert sie und stellt sie über eine einheitliche Schnittstelle sowie ein Dashboard zur Verfügung.

Dieses öffentliche Repository dient als Projektpräsentation und enthält ausgewählte technische Dokumentationen. Der vollständige Quellcode und interne Projektbestandteile bleiben privat.

## Das Problem

Industrielle Maschinen und IoT-Geräte verwenden häufig unterschiedliche Kommunikationsprotokolle. Dadurch entstehen voneinander getrennte Systeme, die sich nur schwer gemeinsam überwachen und verwalten lassen.

## Die Lösung

Protocolbridge verbindet verschiedene Datenquellen in einer gemeinsamen Architektur:

```text
Modbus / OPC UA / MQTT
          ↓
       Gateway
          ↓
      MQTT Broker
          ↓
TimescaleDB und FastAPI
          ↓
  React-Echtzeit-Dashboard
