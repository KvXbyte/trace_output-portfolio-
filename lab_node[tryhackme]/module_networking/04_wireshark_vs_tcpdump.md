# 🧪 Wireshark vs Tcpdump: Packet Analysis Tools

## Covered Topics:
- Interface selection and live capture
- BPF filters (`tcp.port == 80`, `ip.addr == x.x.x.x`)
- Visualization in Wireshark vs CLI output from Tcpdump
- Exporting `.pcap` files

## Key Notes:
- Tcpdump is faster and CLI-based—ideal for headless systems
- Wireshark provides detailed analysis with protocol dissection and stream following
- BPF filters apply at capture time, display filters apply post-capture (in Wireshark)

---

> Raw packets don’t lie. Whether visual or terminal-based, reading them is your edge.
