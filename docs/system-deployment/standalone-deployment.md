# Standalone Deployment

 Standalone deployment is the most fundamental method of deploying VC Hub. The configuration for a standalone deployment is very simple, and other more complex deployment methods are based on this basic approach.

 In a standalone deployment, VC Hub is installed on a single server. This VC Hub node can connect to multiple PLCs, OPC UA servers, and databases. The VC Hub system in standalone deployment can use the built-in SQLite database to store historical data, or it can connect to other database servers and store historical data within them. Additionally, this server allows any number of clients to access it remotely.

<img width="1758" height="1138" alt="image" src="https://github.com/user-attachments/assets/98724b3e-d4a0-49c9-9e24-57694ce61f19" />


#### **Multi-network Support**

 VC Hub supports multi-NIC (Network Interface Card) servers and can act as a bridge between multiple networks or communicate with multiple sites via an enterprise-widearea network. Since clients communicate with the databases and programmable logic controllers (PLCs) through VC Hub, they can launch from both the enterprise network and the isolated control network, providing full access to both. The built-in security settings can restrict access to certain parts of the project or deny access to the entire project based on user roles and network locations, limiting project access to users on different networks.

<img width="1788" height="1160" alt="image" src="https://github.com/user-attachments/assets/03824a4f-e77f-4654-801c-ecddfc2456cd" />





  

  




  

  




 
 

