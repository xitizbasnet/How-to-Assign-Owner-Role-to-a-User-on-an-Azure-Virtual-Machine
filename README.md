# How-to-Assign-Owner-Role-to-a-User-on-an-Azure-Virtual-Machine
How to Assign Owner Role to a User on an Azure Virtual Machine

---

# 📌 1. Purpose

This document provides a structured, step-by-step procedure for assigning **Owner** access to a user for a specific Azure Virtual Machine (VM).

The **Owner** role grants:

* Full administrative permissions
* Ability to manage resources
* Permission to delegate access to other users
* High-level privileged control over the VM

> ⚠️ **Important:** The Owner role is highly privileged. Assign only when operationally required.

---

# ✅ 2. Prerequisites

Before proceeding, ensure the following requirements are met:

* 🔐 You have **Owner** or **User Access Administrator** privileges.
* 👤 The target user exists in Azure Active Directory (AAD).
* 📧 You have the user's AAD email address.
* 🌐 You are signed in to the Azure Portal.
* 🖥️ The target Virtual Machine already exists.

---

# 🔐 3. Procedure

---

## 3.1 🌐 Login to Azure Portal

1. Open your browser.
2. Navigate to:

```
https://portal.azure.com
```

3. Enter your credentials.
4. Successfully log in to the Azure Portal dashboard.

---

## 3.2 🖥️ Navigate to Virtual Machines

1. From the Azure Portal Home page, click:

> **Virtual Machines**

2. The list of available Virtual Machines will appear.

3. Select the VM to which you want to assign access.
   Example: **TRAININGSRV**

4. The selected VM dashboard will open.

---

## 3.3 🔑 Access Control (IAM)

1. In the left-side navigation panel of the selected VM, click:

> **Access control (IAM)**

2. On the top menu bar, click:

> **+ Add**

3. From the dropdown, select:

> **Add role assignment**

---

## 3.4 ➕ Add Role Assignment

1. The **Add role assignment** panel will open.

2. Under role categories:

   * Select the tab:

     > **Privileged administrator roles**

   * From the available list, choose:

     > **Owner**

3. Click:

> **Next**

to proceed to the member selection stage.

---

## 3.5 👤 Assign Privileged Role

1. Click:

> **+ Select members**

2. A pop-up panel will appear on the right side.

3. In the search field, enter the user’s email address.
   Example:

```
xitiz.basnet@xitiztechservices.com.np
```

4. Select the appropriate user from the search results.

5. Click:

> **Select**

6. Confirm the selected user appears under:

> **Selected members**
> Example: **Xitiz Basnet**

7. Click:

> **Next**

to continue.

---

## 3.6 ✔️ Review and Confirm Access

1. Under **Settings**, ensure the following option is selected:

> Allow user to assign all roles (highly privileged)

2. Click:

> **Review + assign**

3. Carefully review all role assignment details:

   * Role: Owner
   * Scope: Selected Virtual Machine
   * Assigned User

4. Click:

> **Review + assign**

again to finalize the role assignment.

---

# 📬 4. Confirmation

After successful role assignment:

* A confirmation notification will appear on the right-hand side:

  > **Added Role Assignment**

### Verification (Optional but Recommended)

To verify:

1. Ask the assigned user to log in.
2. Confirm they can access and manage the specified VM.
3. Validate role visibility under:

   > Access Control (IAM) → Role assignments

---

# 🏁 5. End of Procedure

Owner access has now been successfully granted to the selected user.

---

# 🔒 Security Reminder

The **Owner** role provides full administrative rights including permission delegation.
Follow your organization's least privilege principle before assigning this role.

---

### *** END OF DOCUMENT ***
