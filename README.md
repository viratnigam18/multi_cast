# MultiCast 📺

**MultiCast** is a high-performance, cross-platform local P2P screen sharing application. It enables seamless screen casting across Windows, macOS, iOS, and Android devices over local networks.

---

## 🏗️ Architecture

MultiCast uses a decentralized P2P architecture to minimize configuration and maximize performance:

- **Discovery (mDNS/Bonjour):** Automatically discovers peers on the local network. No manual IP entry required.
- **Signaling (WebSockets):** Handles the exchange of SDP and ICE candidates to set up connections.
- **Transport (WebRTC):** Streams screen and audio data peer-to-peer with low latency and high throughput.

## ⚙️ Network Requirements

For optimal connectivity, ensure the following:
1. **Same LAN:** All devices must be on the same local network (Wi-Fi or LAN).
2. **mDNS Support:** Your router/switch must allow Multicast DNS traffic.
3. **No Isolation:** "AP Isolation" or "Client Isolation" must be disabled on your router.
4. **Firewall Access:** Allow traffic for WebRTC UDP ports and the signaling server's TCP port.

---
*Built for fast, secure, and zero-config local screen broadcasting.*
