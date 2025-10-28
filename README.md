# 🦺 Safety Tracking App — ServiceNow  

A lightweight **ServiceNow application** that allows users to **log, track, and manage safety issues** through a clean **Service Portal** interface.  
Built to demonstrate how simple components — a table, a record producer, a flow, and a UI policy — can work together to automate safety reporting.  

---

## 🚀 Overview  

The **Safety App** lets employees or users easily report safety incidents within the organization.  
Once submitted, each issue is automatically recorded, assigned, and tracked in real-time through a custom Service Portal.  

This project was created to showcase:  
- Practical use of **ServiceNow app development fundamentals**  
- The power of **low-code automation** via Flow Designer  
- A focus on **simplicity and usability** for non-technical end users  

---

## 🧩 Features  

| Feature | Description |
|----------|--------------|
| 🗂️ **Custom Table** | Stores all safety issue records with unique identifiers and categorized fields. |
| 📝 **Record Producer** | Provides a user-friendly submission form for logging new safety issues. |
| 🌐 **Service Portal** | Lists all existing issues and includes a “Create Safety Issue” button for easy access. |
| ⚙️ **Flow Designer Automation** | Automatically assigns issues and sends notifications when specific categories are selected. |
| 🔒 **UI Policy** | When a record’s **State = Closed**, related fields become read-only to maintain data integrity. |
| ✅ **Confirmation Page** | Displays a success message after submission, returning users to the list view. |

---

## 🧠 How It Works  

1. **User opens the Service Portal**  
   → Views all logged Safety Issues in a list widget.  

2. **Click “Create Safety Issue”**  
   → Opens the Record Producer with predefined fields (e.g., Category, Description, State).  

3. **Submit the form**  
   → Confirmation message appears (“Submitted successfully”).  

4. **Flow Designer triggers**  
   → If *Category = Big*, the issue auto-assigns to the **Service Desk Manager** and sends a notification.  

5. **UI Policy enforcement**  
   → When the record is marked **Closed**, most fields become read-only.  

---

## 🧰 Technical Components  

| Component | Type | Description |
|------------|------|-------------|
| **x_safety_issue** | Table | Stores all issue data |
| **Record Producer** | Catalog Item | Captures user input for new records |
| **Flow: Safety Assignment Flow** | Flow Designer | Handles assignment & notifications |
| **UI Policy: Lock Fields on Close** | UI Policy | Enforces read-only state rules |
| **Service Portal: Safety Portal** | Portal Page | Displays list & create button |
| **Widget(s)** | Portal Widgets | Used for listing records & submission navigation |

---
## 📸 Demo Preview  

🎥 *Watch the short demo video on LinkedIn or inside this repository’s media folder.*  
Shows:  
- Portal listing  
- Record creation  
- Confirmation page  
- UI Policy in action  
- Flow automation execution  

---

## ⚡ Setup Guide  

1. **Clone or Download** this repository.  
2. Import the **Update Set** (`Safety_App_Update_Set.xml`) into your ServiceNow instance.  
3. Preview and Commit the update set.  
4. Navigate to your **Service Portal** → “Safety Portal.”  
5. Test by submitting a new record and observe Flow execution.  
---

## 📚 Learning Takeaways  

- Small automations can make a big difference in user experience.  
- Record Producers and Flows are powerful entry points for real-world ITSM use cases.  
- Simplicity often leads to maintainability — fewer parts, cleaner logic.  

---

## 👨‍💻 About the Developer  

**Edgar Quindao Jr.** — Aspiring ServiceNow Developer | ITSM Enthusiast  
📧 Contact: quindaoedgar122217@gmail.com  
🔗 LinkedIn: https://www.linkedin.com/in/edgar-quindao-jr-31a934301/
🔗 GitHub: https://github.com/EdQuinJr

---

## 🏷️ Tags  

`#ServiceNow` `#ITSM` `#LowCode` `#Automation` `#FlowDesigner` `#ServicePortal` `#UIpolicy`
