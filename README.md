# Firebase Project Setup: SaubonLaundryEssentials

This repository contains the setup documentation for the **SaubonLaundryEssentials** Firebase project, demonstrating the configuration of both **Cloud Firestore** and **Realtime Database** with test mode security rules.

---

## 📁 **Screenshots Documentation**

### **1. Cloud Firestore Setup**
| File | Description | Verification |
|------|-------------|--------------|
| `firestore-data.png` | Shows the `SaubonLaundryEssentials` collection containing the `SaubonLaundryEssentials_Logs` document with test data. | ✅ Document fields include: `Accuracy` (Number), `ClassType` (String), `Time` (String), `Date` (String) |
| `firestore-rules.png` | Firestore security rules configured in **test mode** for development. | ✅ Rules are set to: `allow read, write: if true;` |

### **2. Realtime Database Setup**
| File | Description | Verification |
|------|-------------|--------------|
| `realtime-db-data.png` | Default empty view of the Realtime Database. | ✅ Database URL shows correct location: `asia-southeast1` |
| `realtime-db-rules.png` | Realtime Database security rules with **auto-expiring test mode**. | ✅ Rules allow read/write until: `2026-01-12` (timestamp: 1768147200000) |

---

## 🔧 **Technical Specifications**

### **Firestore Configuration**
- **Collection ID:** `SaubonLaundryEssentials`
- **Document ID:** `SaubonLaundryEssentials_Logs`
- **Document Fields:**
  - `Accuracy`: 100 (Number)
  - `ClassType`: "row class" (String)
  - `Time`: "1:20 PM" (String) - Philippine time at setup
  - `Date`: "Enero 17, 2025" (String) - Philippine date at setup

### **Security Rules Status**
| Database | Mode | Expiry | Status |
|----------|------|--------|--------|
| **Firestore** | Test Mode | None | ✅ Active |
| **Realtime DB** | Test Mode | January 12, 2026 | ✅ Active |

---

## 📍 **Project Details**
- **Project Name:** SaubonLaundryEssentials
- **Firebase Region:** Singapore (asia-southeast1)
- **Setup Date:** January 17, 2025
- **Setup Time:** Approximately 1:20 PM (PHT)

---

## 🚀 **Next Steps for Production**
1. Replace test mode security rules with proper authentication-based rules
2. Implement proper data structure for laundry essentials inventory
3. Set up Firebase Authentication for user management
4. Configure Firebase Storage for product images

---

## 📄 **Submission Compliance**
✅ All 4 required screenshots are included  
✅ Both databases are properly configured  
✅ Security rules are in test mode as required  
✅ Project naming follows specification: `LastName_ClassType` format  

---

*This setup was completed as part of backend services and APIs coursework.*
