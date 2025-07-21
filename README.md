# 🔥 Firewall as a Service (FWaaS)

## 📋 Λόγοι σχεδίασης της λύσης
- Κεντρική, διαχειριζόμενη υπηρεσία ασφάλειας για όλους τους φορείς
- Χωρίς ανάγκη επένδυσης σε τοπικό εξοπλισμό ασφαλείας από τους φορείς
- Δεν απαιτείται εξειδικευμένο προσωπικό για υποστήριξη και διαχείριση
- Υψηλή διαθεσιμότητα μέσω γεωγραφικής κατανομής
- Κεντρική διαχείριση πολιτικών και ρυθμίσεων μέσω FortiManager
- Monitoring και reporting μέσω FortiAnalyzer
- **Managed Service μοντέλο**: Ασφάλεια «χωρίς κόπο» για τον φορέα
- Ευελιξία και επεκτασιμότητα για φορείς κάθε μεγέθους

---

## 🖥️ Οικοσύστημα υποδομής
- 2 x FortiGate 5144C chassis
- 4 x FortiGate 5001D blades (Active-Standby)
- FortiManager VM
- FortiAnalyzer VM

---

## 🔐 Χαρακτηριστικά υπηρεσίας
- Stateful Firewalling
- Intrusion Prevention System (IPS)
- DoS/DDoS Mitigation
- Anti-Malware/Antivirus
- Application Control
- Static URL Filtering
- VPN Remote Access
- Data Loss Prevention (DLP)

---

## 📝 Παράδοση υπηρεσίας
1️⃣ Αίτημα φορέα ➔ ΕΔΥΤΕ  
2️⃣ Δημιουργία Virtual Firewall (VDOM) στο FortiGate  
3️⃣ Σύνδεση φορέα μέσω FortiManager (Radius Authentication)  
4️⃣ Διαχείριση πολιτικών προστασίας από τον φορέα  
5️⃣ Πρόσβαση στα εργαλεία monitoring μέσω FortiAnalyzer

---

## ⚙️ FortiManager
- **Policy & Objects**: Διαχείριση πολιτικών ασφαλείας
- **VPN Manager**: Οπτική διαχείριση VPNs
- **Fabric View**: Απεικόνιση του συνολικού δικτύου

---

## 📊 FortiAnalyzer
- Security Operations Center (SOC) δυνατότητες
- Πλήρης ανάλυση logs
- Παρακολούθηση Incidents & Events
- Advanced reporting

---

## 🖧 Αρχιτεκτονική Topology Overview
> CE Router ➔ PE Router ➔ FortiGate Firewall ➔ Internet  
> Υποστήριξη inside/outside zones ανά φορέα, BGP peering, VRFs ανά οργανισμό

---

## 🛡️ High Availability & DDoS Mitigation
- Device failover, Link failover, Session failover
- Virtual MAC addressing με ARP updates για seamless recovery
- Arbor Sightline για ανίχνευση & mitigation επιθέσεων
- Manual & automatic mitigation flows
- Υποστήριξη future expansion: scrubbing routers, API integration

---

## 🚀 Closing
> Η λύση FWaaS του ΕΔΥΤΕ προσφέρει ασφάλεια, διαθεσιμότητα, ευκολία και απλοποίηση της διαχείρισης, χωρίς επιπλέον κόστος ή προσπάθεια από τους φορείς.

