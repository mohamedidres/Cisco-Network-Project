# 🎓 University Campus Network Design

This project is a complete network design for a **university campus**, created using **Cisco Packet Tracer**, implementing both logical and physical topology designs with proper IP addressing and routing protocols.

---

## 📚 Description

The project simulates a real-world campus environment with the following structure:

- **4+ faculties**, each with:
  - **4 floors**
  - Each floor has **5 labs**
  - Each lab includes **10 PCs**
  - Lab PCs are connected in **mesh and star topology** via switches
- **Each floor's switches** are connected to a **floor switch**
- All floors are connected via a **main switch** that connects to the **University router**
- A **Scientific Computation Center**:
  - Includes **multiple servers**
  - All connected via a dedicated switch
- A **main router** connects:
  - All faculties
  - The Scientific Computation Center
  - The outside world (Internet)

---

## 🔧 Technical Implementation

- 🔄 **Routing Protocol**: Implemented **RIP (Routing Information Protocol)** to manage routing between faculties and the Scientific Computation Center  
- 🌐 **IP Addressing**: Used **Classless Inter-Domain Routing (CIDR)** to distribute public IPs efficiently to all sub-networks  
- 📶 **VLAN Configuration**: VLANs are applied and tested to isolate traffic between departments/faculties  
- 🔌 **Topologies Used**:
  - **Star topology** in lab core connections
  - **Mesh topology** for redundancy in lab PCs

---

## 🧪 Test Scenarios

### 🔹 Scenario 1:
- **Source**: PC 0 – First floor, Lab 2, Faculty of Computers & AI  
- **Destination**: Server 0 – Scientific Computation Center  
- **Goal**: Access academic data repository  
- ✅ *Successfully tested*

### 🔹 Scenario 2:
- **Faculty-to-Faculty Communication**: PC from Faculty of Engineering accessing shared resources from Faculty of Science  
- ✅ *Successfully tested through VLAN & RIP routes*

### 🔹 Scenario 3:
- **Internet Access Simulation**: PC in Faculty of Medicine accessing external server via main router  
- ✅ *Route traced and verified using RIP and default routing*

### 🔹 VLAN Scenario:
- PCs in different faculties but in the same VLAN are able to communicate  
- PCs in different VLANs are **isolated**  
- ✅ *VLAN verified using simulation mode*

---

## 🗂️ Files Included

- `EL-PROJECT0.pkt`: Main Packet Tracer project file
- `README.md`: Project documentation

---

## 🛠️ Tools Used

- Cisco Packet Tracer
- RIP Protocol
- CIDR (Classless IP addressing)
- VLAN configuration
- Mesh & Star topologies

---

## 👨‍💻 Author

Mohamed Idres  
Student at Zewail City of Science and Technology  
📍 Egypt

---

## 📎 Notes

To open the project:
1. Download `EL-PROJECT0.pkt`
2. Open it using **Cisco Packet Tracer v7.2 or later**
3. Use simulation mode to test scenarios

---

## 🏷️ Tags

`#Cisco` `#Networking` `#PacketTracer` `#CampusNetwork` `#VLAN` `#CIDR` `#RIP` `#StudentProject` `#ZewailCity`
