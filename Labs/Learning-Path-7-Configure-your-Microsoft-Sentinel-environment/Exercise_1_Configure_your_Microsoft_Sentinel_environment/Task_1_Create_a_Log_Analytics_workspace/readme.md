# SC-200T00A – Learning Path 7  
## Lab 1 – Exercise 1  
### Task 1 – Create a Log Analytics Workspace

---

## 📌 Objective

Create a **Log Analytics Workspace** in Microsoft Azure to onboard Microsoft Sentinel.

---

## 🏗 Environment

- Platform: Microsoft Azure
- Service: Log Analytics Workspace
- Resource Group: Defender-RG
- Workspace Name: defenderWorkspace
- Region: West US (default)

---

## 🔐 Step 1 – Access the Virtual Machine

1. Log in to the **WIN1** virtual machine.
2. Username: `Admin`
3. Password: `Pa55w.rd`

---

## 🌐 Step 2 – Access Azure Portal

1. Open **Microsoft Edge**.
2. Navigate to:  
   https://portal.azure.com
3. Sign in using the tenant credentials provided by the lab.

---

## 🔎 Step 3 – Navigate to Microsoft Sentinel

1. In the Azure portal search bar, type:

2. Select **Microsoft Sentinel** from the results.

---

## ➕ Step 4 – Create a New Log Analytics Workspace

1. Select **+ Create**.
2. Click **Create a new workspace**.

---

## ⚙ Step 5 – Configure Workspace Settings

### Project Details

- **Subscription:** Azure subscription 1
- **Resource Group:**  
- Click **Create new**
- Enter: `Defender-RG`
- Select **OK**

### Instance Details

- **Name:** `defenderWorkspace`
- **Region:** West US (default)

---

## ✅ Step 6 – Validate and Deploy

1. Select **Review + create**.
2. Wait for validation to pass.
3. Select **Create**.
4. Wait for deployment status to show **Created**.

---

## ✔ Expected Result

A successfully deployed Log Analytics Workspace with the following configuration:

| Setting           | Value               |
|------------------|--------------------|
| Resource Group   | Defender-RG        |
| Workspace Name   | defenderWorkspace  |
| Region           | West US            |
| Status           | Created            |

---

## 🎯 Outcome

The Log Analytics Workspace is now ready for Microsoft Sentinel deployment.

---

