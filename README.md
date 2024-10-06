# Setting Up VirtualBox on Windows

### 1. Description

This project aims to demonstrate how to install Oracle VirtualBox on Windows machine, so that it's easy to follow other guides in this repository.

### 2. Objectives

- Set VirtualBox to run all the home lab projects on.


### 3. Tools and Technologies Used

- **VirtualBox**: Used for creating virtual machines for the lab environment;
- **Windows 11**: Used as a monitored system;

### 4. Installation Steps
First of all, we need to download the executable file of Oracle VirtualBox, so we go <a href="https://www.virtualbox.org/wiki/Downloads">here</a> and we choose the file according to our operating system, her we will be choosing windows. We download the virtualbox executable itself and the VirtualBox Extension Pack, as shown in the image below.

![image](https://github.com/user-attachments/assets/3926968f-b96a-4154-a676-5d24cf2b8e30)

After successfully downloading the files, we will see them on the Download folder as shown below.

<img width="342" alt="image" src="https://github.com/user-attachments/assets/e3e4a01d-7945-436d-8a1c-c19a3cee6999">
<br>
<br>

We'll start by the VirtualBox-version-Win installation, as below.


<img width="382" alt="image" src="https://github.com/user-attachments/assets/5f338569-26cd-4300-9656-93d8eaa29763">



For setting up VirtualBox, refer to <a href="https://github.com/Muhate/Setting-Up-VirtualBox">this guide</a>
<br>
<br>
   
   - **4.2: Setting Up Windows 2022 on VirtualBox**

For setting up Windows 2022 on VirtualBox, refer to <a href="https://github.com/Muhate/Install-Windows-on-VirtualBox">this guide</a>
<br>
<br>

   - **4.3: Setting Up Ubuntu Server 24.04.LTS on VirtualBox**

For setting up Ubuntu Server on VirtualBox, refer to <a href="https://github.com/Muhate/Install-Ubuntu-on-VirtualBox">this guide</a>
<br>
<br>

   - **4.3: Setting Up Wazuh Manager on Ubuntu Server 24.04 LTS**

     - Update the package manager:
       ```
       sudo apt update && sudo apt upgrade -y && sudo reboot
       ```
     - Install Wazuh Manager:
       ```
       curl -s https://packages.wazuh.com/4.x/ubuntu/KEY.gpg | sudo apt-key add -
       echo "deb http://packages.wazuh.com/4.x/ubuntu/ focal main" | sudo tee /etc/apt/sources.list.d/wazuh.list
       sudo apt-get update
       sudo apt-get install wazuh-manager
       ```

   - **Step 3: Configuring Wazuh**
     - Modify the configuration file (`/var/ossec/etc/ossec.conf`) to set up agents and alerts.
     - Restart Wazuh Manager:
       ```bash
       sudo systemctl restart wazuh-manager
       ```

   - **Step 4: Installing Elasticsearch and Kibana**
     - Follow similar steps to install and configure Elasticsearch and Kibana.

### 5. **Generating Test Data**
   - **Kali Linux Testing**: 
     - Execute various tests to generate logs (e.g., using Metasploit, Nmap).
     - Sample command to generate logs:
       ```bash
       nmap -sS -p 1-65535 <target_ip>
       ```

### 6. **Results and Analysis**
   - **Data Visualization**: 
     - Showcase screenshots of dashboards in Kibana that display security events, logs, and alerts.
   - **Alerts Configuration**:
     - Explain how alerts were configured in Wazuh and provide examples of alerts generated during testing.

### 7. **Challenges and Solutions**
   - **Challenge**: Difficulty in integrating Wazuh with Elastic Stack.
     - **Solution**: Consulted official documentation and community forums, which helped resolve configuration issues.

### 8. **Lessons Learned**
   - Gained hands-on experience in setting up a complete SIEM solution.
   - Improved understanding of log analysis and incident response workflows.

### 9. **Future Improvements**
   - Plan to integrate additional data sources (e.g., firewalls, web servers).
   - Explore automated incident response mechanisms using Wazuh.

### 10. **Conclusion**
   - This project successfully demonstrated the deployment of Wazuh in a lab environment, providing valuable insights into security monitoring and log analysis.

### 11. **Links and References**
   - [GitHub Repository](https://github.com/username/wazuh-lab)
   - [Wazuh Official Documentation](https://wazuh.com/documentation/)
   - [Elastic Stack Documentation](https://www.elastic.co/guide/en/elastic-stack/current/index.html)

### 12. **Contact Information**
   - **Name**: Rogério Muhate
   - **Email**: rbmuhate@gmail.com
   - **LinkedIn**: [LinkedIn Profile](https://www.linkedin.com/in/rmuhate)
