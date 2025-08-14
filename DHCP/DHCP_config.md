# DHCP

- Installed and configured the DHCP server role on Windows server
- Set and activated DHCP scope
- Tested and made sure client recieved automatic IP assignement, verified lease allocation and reservation functionality

  DHCP Server set up with a single scope of 172.16.0.100-200, DNS: 172.16.0.1 (Domain Controller used as DNS), Default Gateway: 172.16.0.1 which is the DC's Ipv4 (Clients will use the internal NIC of the domain controller as the default gateway/router)

  This will allow the Windows 10 Client to automatically get an IP address, which lets them access the internet, regardless of being on this private internal network- similar to an office setting.

  Server Manager > Add Roles and Features Wizard > Install DHCP


   <img width="397" height="454" alt="Server Options DHCP Router" src="https://github.com/user-attachments/assets/82bf30aa-ba53-4c46-aedf-29e61602a684" />


  <img width="1024" height="478" alt="DHCP Address Pool" src="https://github.com/user-attachments/assets/ba2b324a-2c93-427d-ac50-355147ee3b49" />


    Ensuring the Windows 10 Client was on the list of address leases after creation: 


    <img width="1024" height="435" alt="DHCP Address Leases" src="https://github.com/user-attachments/assets/41210475-a98a-4744-989b-12764f321139" />
