# wireshark-protocol-analysis-task5
# Wireshark Packet Capture Analysis - Task 5

## Objective
The goal of this task was to capture live network traffic using Wireshark and identify basic protocols and traffic types.

---

## Steps Performed

✅ Installed Wireshark on my system  
✅ Started a packet capture on my active network interface  
✅ Generated traffic by browsing websites and pinging external servers  
✅ Stopped the capture after ~1 minute  
✅ Used filters in Wireshark to analyze captured packets by protocol  
✅ Identified at least 3 different protocols  
✅ Exported the `.pcapng` file and documented my findings

---

## Protocols Identified

1. **DNS (Domain Name System)**  
   - Queries and responses for domain name resolution (e.g., Google, Instagram, YouTube, Facebook).  
   - Example filter used: `dns`

2. **TCP (Transmission Control Protocol)**  
   - Connections established for secure data transfer (HTTPS), including 3-way handshake, data exchange, ACKs, FINs.  
   - Example filter used: `tcp`

3. **ICMP (Internet Control Message Protocol)**  
   - Echo (ping) requests and replies, showing reachability tests.  
   - Example filter used: `icmp`

4. **TLS (Transport Layer Security)** / **QUIC**  
   - Encrypted communication for HTTPS connections, including TLS handshakes and encrypted payloads.  
   - Example filter used: `tls` or `quic`

---

## Key Findings

- My device (**192.168.1.35**) communicated with several external servers (e.g., **114.79.129.2**, **142.250.183.78**, **104.17.118.12**).
- **DNS** queries revealed domain names like `accounts.google.com`, `assets.msn.com`, `play.google.com`, and others.
- **TCP** traffic included normal handshake sequences (SYN, SYN-ACK, ACK), data exchange, and graceful terminations (FIN, ACK).
- **ICMP** traffic confirmed active ping tests with echo requests and replies.
- **TLS/QUIC** traffic showed encrypted HTTPS/QUIC sessions (cannot be decrypted without appropriate keys).

---

## Commands/Filters Used in Wireshark

- **Filter DNS packets:**
- **Filter TCP packets:**  
- **Filter ICMP packets:**  
- **Filter TLS traffic:**  
- **Filter QUIC traffic:**
---

## Deliverables

📁 `task5_capture.pcapng` (📥 [Download Capture File](https://drive.google.com/file/d/1fefYSNhrEPqaYPEbARViSqc45PLgqujk/view?usp=drive_link)
 
📝 This `README.md` file summarizing the analysis and findings

---

## Conclusion

This exercise improved my hands-on skills in:
- Using Wireshark for live packet capture  
- Filtering and analyzing captured packets by protocol  
- Understanding different traffic types in typical network usage  
- Gaining awareness of encrypted vs. unencrypted protocols

---

**Author:**  
Yadidiah Sangem  



 
