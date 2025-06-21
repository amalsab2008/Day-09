# 🛡️ Day 09 - Cybersecurity: Wireshark Overview

## 📘 What is Wireshark?
Wireshark is a powerful, open-source network protocol analyzer. It captures and displays data packets traveling through a network in real-time, allowing users to examine the traffic in detail. It’s widely used by network administrators, security professionals, and developers.

---

## 💻 Platforms Supported
- **Windows**
- **Linux** (and other Unix-like systems)
- **macOS**

Wireshark is cross-platform and offers both a graphical user interface (GUI) and a command-line interface through its `tshark` tool.

---

## 🎯 Purpose of Wireshark
Wireshark is mainly used for:
- Network troubleshooting
- Analyzing network performance
- Detecting network intrusions
- Learning protocol internals
- Ethical hacking and penetration testing
- Debugging network-related software

---

## ⚙️ Main Functions of Wireshark
- **Packet Capturing**: Records real-time data packets on a network interface.
- **Protocol Analysis**: Understands and decodes hundreds of protocols (TCP, UDP, HTTP, FTP, DNS, etc.).
- **Filtering**: Supports advanced display and capture filters to focus on specific traffic.
- **Exporting Data**: Captured data can be saved and exported in various formats (e.g., .pcap, .csv, .txt).
- **Color Coding**: Highlights different types of packets for better visibility.
- **Follow Streams**: Reconstructs and displays complete conversations like HTTP requests/responses.

---

## 🧑‍💻 How to Use Wireshark
1. **Install Wireshark** on your system.
2. **Launch the application**.
3. **Select the network interface** to monitor (e.g., Ethernet, Wi-Fi).
4. **Start capturing packets**.
5. **Use display filters** like:
   - `ip.addr == 192.168.0.1` (filter by IP)
   - `tcp.port == 80` (filter by port)
   - `http` (only show HTTP traffic)
6. **Stop capturing** after you’ve collected enough data.
7. **Analyze packets** by expanding different layers (Ethernet, IP, TCP/UDP, Application Layer).
8. **Save the capture file** if needed for later analysis.

---

## 🧠 Use by Ethical Hackers
Ethical hackers use Wireshark to:
- **Identify plaintext credentials** sent over unencrypted protocols (e.g., FTP, Telnet)
- **Perform reconnaissance** by analyzing devices communicating on the network
- **Detect vulnerabilities** by monitoring outdated or vulnerable protocols in use
- **Capture handshake data** for offline password cracking (e.g., WPA2 handshakes)
- **Audit traffic** to detect policy violations and data exfiltration

🔐 **Important:** Always have permission when performing packet captures on any network.

---

## ⬇️ How to Download Wireshark
### 🔸 On Windows:
1. Visit: [https://www.wireshark.org/download.html](https://www.wireshark.org/download.html)
2. Download the Windows installer
3. Run the installer and follow instructions
4. Ensure you install **Npcap** (necessary for packet capturing)

### 🔸 On Linux:
```bash
# For Debian/Ubuntu-based distributions:
sudo apt update
sudo apt install wireshark

# For Fedora:
sudo dnf install wireshark-qt

# For Arch:
sudo pacman -S wireshark-qt
```
You may need to add your user to the `wireshark` group:
```bash
sudo usermod -aG wireshark $USER
```
Then restart your session.

---

## 📌 Real-World Scenarios
1. **Troubleshooting a Slow Network**:
   - Detect which IP or service is generating excessive traffic
2. **Identifying Malware Activity**:
   - Spot communication to suspicious domains or IPs
3. **Unauthorized Device Detection**:
   - See if unknown MAC/IPs are accessing your network
4. **Capturing Credentials in Training Labs**:
   - Ethical hackers can demonstrate risks of using unencrypted services
5. **Application Debugging**:
   - Developers can trace bugs related to networking code
6. **Forensic Investigations**:
   - Analyze captured traffic after a security incident

---

## ✅ Conclusion
Wireshark is an essential tool in the field of cybersecurity, offering visibility into what's happening at a microscopic level in a network. Whether you are troubleshooting, analyzing threats, or learning network protocols, mastering Wireshark is a valuable step for any aspiring cybersecurity professional.

---

📎 **Reminder**: Always use tools like Wireshark responsibly and with the appropriate authorization. Unauthorized packet capturing is illegal and unethical.
