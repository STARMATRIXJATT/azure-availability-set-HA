# Azure Availability Set with Linux VMs (Day 23 - #100DaysOfCloud)

This project demonstrates how to create a **Managed Availability Set** and deploy **Linux Virtual Machines (Ubuntu LTS)** inside it using the Azure Portal & Azure Cloud Shell.

---

## 💡 What you will do:

- Create a Managed Availability Set
- Generate a 4096-bit RSA SSH Key Pair using Cloud Shell (Bash)
- Deploy 2 Ubuntu Virtual Machines within the Availability Set
- Verify distribution across Fault & Update Domains for high availability

---

## 🚀 Steps

### 1️⃣ Create a Managed Availability Set
- Resource Group: `rg1lod49580678`
- Availability Set Name: `app-frontend-avset`
- Fault Domains: **2**
- Update Domains: **5**
- Managed Disks: **Yes (Aligned)**

---

### 2️⃣ Open Cloud Shell and Generate SSH Keys
```bash
ssh-keygen -t rsa -b 4096 -q

---

### 3️⃣ Display Public Key
```bash
cat ~/.ssh/id_rsa.pub
