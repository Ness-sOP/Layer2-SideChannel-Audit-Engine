# Layer-2 Side-Channel & Infrastructure Pivoting Audit Engine
### 🚀 Developed by: Ness_uOP (Micro-Operations & Protocol Research)

A production-grade network exploration and protocol auditing suite written in Python/Scapy. This framework is specifically engineered to navigate hardened virtualized environments and dynamically pivot from silent endpoint micro-timing diagnostics to local infrastructure traversal and traffic interception.


## 🛠️ Core Architectural Modules

The engine operates across four distinct abstraction layers to profile local segments without relying on open application-layer socket states:

1. **Pre-Warmed Hardware CPU Governor Jitter Analyzer**  
   Fires precision Layer-2 timing loops to stabilize mobile power-saving governors before executing packet bursts. This isolates true kernel scheduler queue delays from CPU clock acceleration noise, exposing hidden filtering hooks.

2. **Finite TCP Zero-Window State Clamping**  
   Combines asynchronous connection-priming sequences with zero-window flow control parameters to measure structural state-table lookup latencies inside the target operating system's network driver.

3. **Infrastructure Pivot & Variable Harvesting**  
   Bypasses virtual host adapter driver boundaries (such as containerized or mirrored networking constraints) by shifting to stateful, thread-pooled socket abstractions. Successfully queries open infrastructure gateways to extract unauthenticated client-side firmware parameters and carrier-specific runtime logic.

4. **Layer-2 Topology Manipulation Platform**  
   Abuses the intrinsic design boundaries of unauthenticated local protocols through high-velocity CAM table starvation routines (MAC Flooding) and continuous, asynchronous ARP cache alignment loops to evaluate local segment routing dependency and fallback resilience.

---

## 📋 Implemented Methodologies (Bilingual Matrix)

| English Description | Descripción en Español |
| :--- | :--- |
| **Stateful TCP Socket Sweeping** | Barrido de Sockets TCP con Seguimiento de Estado |
| **Advanced UDP Port Unreachable Scanning** | Escaneo Avanzado UDP de Puerto No Alcanzable |
| **TCP ACK Firewall Mapping Scan** | Escaneo de Mapeo de Firewall mediante TCP ACK |
| **Application-Layer Banner Grabbing** | Extracción de Banners a Nivel de Aplicación |
| **TCP Simultaneous Open State Machine Probing** | Sondeo de la Máquina de Estados mediante Apertura Simultánea TCP |
| **Micro-Fragmented IPv6 Extension Header Evasion** | Evasión mediante Encabezados de Extensión IPv6 Micro-Fragmentados |
| **Pre-Warmed Hardware CPU Jitter Analysis** | Análisis de Jitter de CPU de Hardware en Estado Pre-Calentado |
| **Finite TCP Zero-Window Data Push Scan** | Escaneo Finito de Empuje de Datos con Ventana Cero TCP |
| **TCP Option Padding Evasion (NOP Influx)** | Evasión por Relleno de Opciones TCP (Inflado de NOPs) |
| **CAM Table Overflow (MAC Matrix Flooding)** | Desbordamiento de Tabla CAM (Inundación de Matriz de MACs) |
| **Asynchronous ARP Cache Table Poisoning** | Envenenamiento Asíncrono de la Tabla de Caché ARP (MitM) |
| **ICMPv6 Multicast Listener Discovery Probing** | Sondeo de Descubrimiento de Escucha Multicast ICMPv6 (MLDv2) |
| **ARP Link-State Mutation Paradox Injection** | Inyección de Paradoja de Mutación del Estado de Enlace ARP |

---

## 🚀 Deployment Instructions

### Prerequisites
The engine utilizes low-level raw socket interfaces which require explicit kernel-level processing privileges and standard packet craft libraries:
```bash
sudo pip3 install scapy
```

### Infrastructure Preparation (For MitM/Pivoting Modules)
To allow the local host kernel to act as a legitimate Layer-3 forwarding node instead of discarding routed transit traffic, you must explicitly enable packet forwarding in your Linux subsystem parameters before launching the loop:
```bash
sudo sysctl -w net.ipv4.ip_forward=1
```

### Running the Engine
Execute the audit cycle using root permissions to allow direct data-link layer frame manipulation over your active interface:
```bash
sudo python3 advanced_fuzzer.py
```

### Safe Environment Teardown
Once the testing cycle concludes, safely restore your host kernel parameters to their default secure state:
```bash
sudo sysctl -w net.ipv4.ip_forward=0
```
