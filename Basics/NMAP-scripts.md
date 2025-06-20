---

### **1. Target Specification**
- `-iL (example.txt)`: Input list of IPs/hosts/networks from file.

---

### **2. Host Discovery**
- `-sL`: List Scan — show targets without scanning.  
- `-sn`: Ping Scan — skip port scanning.  
- `-Pn`: Treat all hosts as online (skip host discovery).

---

### **3. Scan Techniques**
- `-sS`: TCP SYN scan.  
- `-sT`: TCP Connect scan.  
- `-sA`: TCP ACK scan.  
- `-sU`: UDP scan.

---

### **4. Port Specification and Order**
- `-p <ports>`: Scan only specified ports.  
  Examples:  
  - `-p22` (only port 22)  
  - `-p1-65535` (all ports)  
  - `-p U:53,111,137,T:21-25,80,139,8080,5:9` (mixed UDP and TCP)  
- `--exclude-ports <ports>`: Exclude specific ports from scan.  
- `-F`: Fast mode — scan fewer ports than default.  
- `-r`: Scan ports in order (no randomization).

---

### **5. Service/Version Detection**
- `-sV`: Probe open ports for service/version info.  
- `--version-intensity <0–9>`: Set intensity (0=light, 9=exhaustive).  
- `--version-light`: Use common probes (intensity 2).  
- `--version-all`: Try all probes (intensity 9).  
- `--version-trace`: Show detailed scanning progress (for debugging).

---

### **6. Script Scanning (Nmap Scripting Engine)**
- `-sC`: Use default scripts (equivalent to `--script=default`).  
- `--script=<scripts>`: Run specific scripts by name, directory, or category.

---

### **7. Timing and Performance**
- `-T<0–5>`: Timing template (0=paranoid, 5=insane). Higher is faster.

---

### **8. OS Detection**
- `-O`: Enable OS detection.

---

### **9. Output Options**
- `-oN <file>`: Save normal output.  
- `-oX <file>`: Save as XML.  
- `-oS <file>`: Save as script kiddie format.  
- `-oG <file>`: Save in grepable format.  
- `-v`, `-vv`, `-vvv`: Verbosity levels 1 to 3, showing more real-time detail.

---

### **10. Miscellaneous**
- `-A`: Aggressive mode — enables OS detection, version detection, script scan, and traceroute.

---
