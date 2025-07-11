# Network Scan Report

## Target Scanned
- IP Address: 192.168.1.7

## Scan Type
- TCP SYN Scan (-sS)

## Open Ports Found
- 9200/tcp - Unknown service

## Analysis
- Port 9200 is often used by Elasticsearch.
- If Elasticsearch is running and exposed without protection, it can be exploited.
- Recommendation: Restrict access to this port or secure the service.

## Tools Used
- Nmap (v7.95)
- OS: Kali Linux

## Scan Command
```bash
nmap -sS 192.168.1.7 -oN scan_results.txt
