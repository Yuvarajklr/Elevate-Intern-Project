
# 🛡️ Task 5: Capture and Analyze Network Traffic Using Wireshark

## 📌 Objective
The goal of this task is to capture live network traffic using *Wireshark* and analyze it to identify different network protocols. This will help in understanding how data flows through a network and how to troubleshoot network issues effectively.

---

## 🧰 Tools Used
- *Wireshark*: A free and open-source packet analyzer used for network troubleshooting and analysis.
- *Operating System*: [Kali Linux]

---

## 📁 Deliverables
- ✅ Packet capture file: task5-capture.pcap
- ✅ This README.md report

---

## 🧪 Step-by-Step Process

### 1. Go to Wireshark
Downloaded and installed Wireshark from the official website: [https://www.wireshark.org/](https://www.wireshark.org/) or
'/usr/share/applications/org.wireshark.Wireshark.desktop'
### 2. Started Packet Capture
- Opened Wireshark.
- Selected my active network interface (Wi-Fi).
- Clicked *Start Capturing*.

### 3. Generated Network Traffic
To generate traffic:
- Opened a web browser and visited: https://example.com
- Also pinged a server using:
- Go to terminal and prompt such as [ping tryhackme.com]

### 4. Stopped Capture
- Waited approximately 1 minute after browsing and pinging.
- Clicked the Stop button in Wireshark.

### 5. Filtered by Protocol
Used Wireshark filters to isolate specific traffic types:
- HTTP: http
- DNS: dns
- TCP: tcp

### 6. Identified Protocols
Found and analyzed the following protocols:
- 1. DNS – Used to resolve domain names to IP addresses.
- 2. HTTP – Used for transferring web pages.
- 3. TCP – A transport protocol providing reliable data transfer.

### 7. Exported Capture File
Saved the captured traffic using:
- File > Export Specified Packets...
- File name: task5-capture.pcap

### 8. Summarized Findings
- The capture revealed successful DNS lookups for visited websites.
- HTTP packets showed web page requests and responses.
- TCP was the underlying transport layer for most connections.
- Analyzed packet details like source/destination IP, ports, and flags.
