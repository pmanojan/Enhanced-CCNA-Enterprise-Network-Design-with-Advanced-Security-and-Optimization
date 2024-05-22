### Scenario: Network Design for ABC Pvt Ltd, Sri Lanka

ABC Pvt Ltd, a leading enterprise based in Sri Lanka, has its head office located in Colombo. The organization is structured into 12 distinct departments: Marketing, Management, Accounting, Research, Finance, HR, Admin, IT, Staff, Customer, Guest, and Logistics. Each department requires secure and efficient network connectivity to ensure seamless operations.

#### Network Infrastructure

**IP Address Allocation:**
ABC Pvt Ltd has been allocated two network ranges: 192.168.10.0/24 and 192.168.11.0/24. These IP addresses will be distributed among the departments, with a maximum of 28 users per department to ensure sufficient address space and network efficiency.

**Website and Mail Server:**
The company hosts a corporate website and maintains a dedicated mail server. However, access restrictions are in place to enhance security:
- Guests and customers are prohibited from using the company's mail address domain (@abc.lk).
- Only internal staff can use the mail server for company communications.

**Network Segmentation and Security:**
- The Admin department has unique privileges, allowing them to ping and communicate with all other departments. Conversely, no other department can ping or initiate communication with the Admin department, ensuring a controlled and secure administrative environment.
- Each department operates within its own VLAN, ensuring isolation and enhanced security.

**Internet Service Providers:**
To guarantee uninterrupted internet access, ABC Pvt Ltd utilizes two ISPs:
1. **Telecom (Primary ISP)**
2. **Dialog (Backup ISP)**

In case of any connectivity issues with Telecom, Dialog automatically takes over, providing redundancy and high availability.

#### Technical Details

1. **Routing and Redundancy:**
   - **HSRP (Hot Standby Router Protocol)** is implemented to ensure high availability of network gateways.
   - **OSPF (Open Shortest Path First)** is used for efficient routing within the network.

2. **Access Control:**
   - **ACLs (Access Control Lists)** are configured to enforce the communication policies, particularly the restrictions on pinging between departments and the use of the mail server.
   
3. **Network Services:**
   - **DHCP** is utilized for dynamic IP address allocation, simplifying network management.
   - **Syslog Server** is set up for centralized logging and monitoring of network activities.
   - **NTP Server** ensures synchronized time across all network devices.
   - **EtherChannel** is configured for link aggregation, providing increased bandwidth and redundancy.
   - **VLAN & VTP (VLAN Trunking Protocol)** are used to manage and propagate VLAN information efficiently across the network switches.

4. **User Experience:**
   - **Website:** The company's website is accessible to all users, providing necessary information and services.
   - **Mail Server:** Only internal staff can access the company's mail server, while guests and customers are restricted to ensure security and proper use of resources.

This comprehensive network design ensures that ABC Pvt Ltd’s operations are secure, efficient, and resilient, supporting the organization’s growth and providing robust connectivity for all its departments. If you need assistance with similar network designs or have any inquiries, please feel free to contact me.
