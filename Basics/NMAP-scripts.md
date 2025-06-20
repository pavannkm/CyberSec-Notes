# 🛠️ Nmap Commands

---

## **1. Target Specification**
- `-iL <inputfilename>`: Load targets from a file.

---

## **2. Host Discovery**
- `-sL`: List Scan — shows targets without scanning them.
- `-sn`: Ping Scan — skip port scan.
- `-Pn`: Treat all hosts as online (skip host discovery).

---

## **3. Scan Techniques**
- `-sS`: TCP SYN scan.
- `-sT`: TCP Connect scan.
- `-sA`: TCP ACK scan.
- `-sU`: UDP scan.

---

## **4. Port Specification and Order**
- `-p <ports>`: Scan specific ports.  
  Examples:
  - `-p22`
  - `-p1-65535`
  - `-p U:53,111,137,T:21-25,80,139,8080,5:9`
- `--exclude-ports <ports>`: Exclude certain ports.
- `-F`: Fast mode — scan fewer ports.
- `-r`: Scan ports in order (disable randomization).

---

## **5. Service/Version Detection**
- `-sV`: Probe open ports for version info.
- `--version-intensity <0–9>`: Set intensity level.
- `--version-light`: Use common probes (intensity 2).
- `--version-all`: Use all probes (intensity 9).
- `--version-trace`: Show detailed scan process.

---

## **6. Script Scanning (NSE)**
- `-sC`: Run default scripts.
- `--script=<scripts>`: Run specific scripts or categories.

---

## **7. Timing and Performance**
- `-T<0–5>`: Set speed profile (0=slowest, 5=fastest).

---

## **8. OS Detection**
- `-O`: Enable OS fingerprinting.

---

## **9. Output Options**
- `-oN <file>`: Normal text output.
- `-oX <file>`: XML output.
- `-oS <file>`: "Script kiddie" format.
- `-oG <file>`: Grepable format.
- `-v`, `-vv`, `-vvv`: Verbosity levels for more real-time info.

---

## **10. Miscellaneous**
- `-A`: Aggressive scan — enables OS detection, version detection, script scanning, and traceroute.

---
