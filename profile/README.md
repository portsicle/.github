![banner](https://github.com/user-attachments/assets/10a91044-97a7-4659-95da-9a7fde488a46)

**Portsicle** is a reverse tunneling service that creates a public ingress endpoint for local servers, allowing developers to showcase their locally running applications to clients, stakeholders or to test APIs without deploying.

## Repository overview

### 1. **Portsicle Server**

A free and open-source ngrok alternative to expose local servers online with **Minimal setup & high performance**.

### 2. **Portsicle Client**

Portsicle client allows you to use the Portsicle Server via CLI:

- Direct connection to local services running on your machine.
- Routing and forwarding of HTTP traffic to Portsicle Server.

### 3. **Portsicle Proxy**

A lightweight and flexible HTTP/HTTPS forward proxy server that allows Site access management and advanced network logging at local level.

---

### How Portsicle works:

1. Portsicle operates by establishing a **secure wss tunnel** between your local server and a remote Portsicle server.

2. When you run the Portsicle client on your local machine, it connects to the Portsicle server over a wss connection.

3. Incoming requests to the Portsicle server are then securely forwarded through this tunnel to your local server, and responses are sent back through the same tunnel to the requester.

4. This method ensures that your local server remains protected behind your firewall, while still being accessible via a public URL provided by the Portsicle server.

> **NOTE** that Portsicle is currently designed to work with **production‑build assets** where the files are served statically. There’s no mechanism in the current code to dynamically adjust headers based on the HMR requirements. Hence HMR remains a future scope / enhancement for this project.

## Contribution

We welcome contributions! Feel free to open a pull request or an issue.

---

<a href="https://www.buymeacoffee.com/amitsuthar" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
