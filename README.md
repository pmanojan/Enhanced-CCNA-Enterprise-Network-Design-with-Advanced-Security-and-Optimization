### Scenario for ABC Pvt Ltd's Network Design

**Company Overview:**
ABC Pvt Ltd is a prominent enterprise based in Sri Lanka with its head branch located in Colombo. The company operates across 12 departments: Marketing, Management, Accounting, Research, Finance, HR, Admin, IT, Staff, Customer, Guest, and Logistics. To efficiently manage their internal and external communications, they have implemented a comprehensive network design.

**Network Infrastructure:**
ABC Pvt Ltd has acquired two network ranges for their operations:
- **192.168.10.0/24**
- **192.169.11.0/24**

These IP ranges are distributed among their departments, with a maximum of 28 users per department.

**Web and Mail Services:**
The company hosts its website and maintains an internal mail server. However, only internal users have access to the 'abc.lk' email domain, ensuring that guests and customers cannot use these addresses for external communication.

**Departmental Access and Security:**
Each department is equipped with a separate access point, ensuring isolated and secure connectivity:
- **Admin Department:** Can communicate (ping) with all other departments.
- **Other Departments:** Restricted from pinging the Admin department to enhance security.

**Internet Service Providers:**
ABC Pvt Ltd has implemented a dual ISP setup to ensure uninterrupted internet access:
- **Primary ISP:** Telecom
- **Backup ISP:** Dialog

This dual ISP setup ensures high availability and redundancy for internet connectivity.

**Routing and IP Communication:**
The enterprise uses the **100.100.100.0/24** network for router-to-router communication, streamlining internal routing protocols and enhancing network performance.

**Additional Implementations:**
- **DHCP** for dynamic IP allocation.
- **HSRP** for high availability and redundancy.
- **ACLs** to manage and secure network traffic.
- **OSPF** for efficient routing within the enterprise network.
- **Bandwidth Management** to optimize network performance.
- **Syslog Server** for centralized logging and monitoring.
- **NTP Server** to synchronize time across all network devices.
- **EtherChannel** for increased bandwidth and redundancy.
- **VLANs** and **VTP** to segment and manage network traffic efficiently.

**Security Measures:**
To ensure the security of the network, all access points and communication channels are secured with the latest encryption and authentication protocols. The segregation of the Admin department from other departments' ping capabilities adds an extra layer of security, protecting sensitive administrative operations.

**Conclusion:**
With this robust network design, ABC Pvt Ltd ensures high availability, secure communication, and efficient management across all departments, providing a reliable and secure environment for its operations. This setup supports the company's growth and allows for scalable expansion in the future.

---

This scenario outlines the network design and security measures in place for ABC Pvt Ltd, ensuring clarity and comprehensive coverage of the requirements provided.
