# System Integrity Requirements

## Maturity Level 1

### Install the Latest Stable Version of Any Security-Related Updates on All Network Devices

Install the latest stable version of any security-related updates on all network devices. Latest refers to all updates which were available prior to the internal product testing of the product.

> Ensure that you are monitoring for updates.

> The vendor must use the most recent security updates available at the beginning of the development cycle, or later.

Applies to: Hosted components



### Perform Complete System Backups

Ensure that all of the organization's key systems are backed up as a complete system, through processes such as imaging, to enable the quick recovery of an entire system. On premises products must provide this capability.

> These types of backups should be done prior to each for each type of system used. This allows for quick recovery back to the known good version. Maintaining extra units created from these system backups is another good approach.

Applies to: All



### Ensure Anti-Malware Software and Signatures Are Updated

For systems that support the use of anti-malware software, the product must allow an administrator to perform updates to its scanning engine and signature database.

> Ensure that all anti-malware instances are receiving signature updates. This requires periodic review of devices within the technology system.

Applies to: All



### Configure Devices to Not Auto-Run Content

Configure devices to not auto-run executable code from removable media.

> This helps ensure an attacker cannot insert a malicious device and execute it without having user credentials.

Applies to: Vendor supplied hardware



### Use Port Protectors on Unused Ports

Cover all unused communication ports (e.g. USB, Thunderbolt, HDMI, etc.) on endpoint devices with locks or tamper-evident port protectors to ensure unauthorized devices are not inserted into the device. This must be done prior to delivery to the customer.

Applies to: Provider supplied hardware



## Maturity Level 2

### Establish Secure Configurations

Maintain documented, standard security configuration standards for all authorized operating systems and software such as the CIS Benchmarks.

> Using a vetted configuration standard, identify each component of the technology and its secure configuration standard to use.

Applies to: All



### Deploy Operating System Patches

Ensure operating systems are running the latest security updates provided by the software vendor. Latest refers to all updates which were available prior to the internal product testing of the product.

Applies to: Hosted components



### Deploy Software Patches

Ensure that third-party software on all systems is running the latest security updates provided by the software vendor.

> Latest refers to all updates which were available prior to the internal product testing of the product.

Applies to: All



### Utilize Centrally Managed Anti-Malware Software

Utilize centrally managed anti-malware software to continuously monitor and defend workstations and servers.

> All endpoints in an technology solution must use properly installed and constantly running anti-malware software. Central management allows administrators to enforce this rule.

Applies to: All



### Limit Access to Scripting Tools

Limit access to scripting tools (such as Microsoft PowerShell and Python) to only administrative or development users with the need to access those capabilities.

> technology may make use of these technologies, but access to them should be limited to only the most trusted and protected accounts.

Applies to: All



### Configure Anti-Malware Scanning of Removable Devices

Configure devices so that they automatically conduct an anti-malware scan of removable media when inserted or connected.

> Use of USB devices is very common in systems. Therefore, it is critical that all external devices be scanned for malware prior to use.

Applies to: Vendor supplied or controlled hardware



### Use Standard Hardening Configuration Templates for Databases

For applications that rely on a database, use standard hardening configuration templates.

> CIS Benchmarks are available for various database offerings such as MySQL, SQL Server, and PostgreSQL. Guidance for cloud-based databases are also available.

Applies to: All



## Maturity Level 3

### Implement Automated Configuration Monitoring Systems

Utilize a Security Content Automation Protocol (SCAP) compliant or equivalent configuration monitoring system to verify all security configuration elements, catalog approved exceptions, and alert when unauthorized changes occur.

> This prevents accidental misconfiguration and allows RTPs the ability to prove the component has been properly and securely configured.


### Deploy System Configuration Management Tools

Deploy system configuration management tools that will automatically enforce and redeploy configuration settings to systems at regularly scheduled intervals.

> Where possible, each component should be inspected and updated with the latest known good secure configuration prior to use in any.

Applies to: All



### Enable Operating System Anti-Exploitation Features and Deploy Anti-Exploit Technologies

Enable anti-exploitation features such as Data Execution Prevention (DEP) or Address Space Layout Randomization (ASLR) that are available in an operating system, or deploy appropriate toolkits that can be configured to apply protection to a broader set of applications and executables.

> This applies to servers and other sensitive endpoints.

Applies to: All



### Disable Access to USB Devices Where Possible

Disable the use of USB devices (including Thunderbolt) on a system. This completely removes the risk of removable USB media based attacks.

> This may not be feasible for all components. It should be feasible for servers and other devices which do not use USB connected devices.

Applies to: Vendor provided hardware




### No Single Points of Failure

Protect product reliability against any one system component failing by providing redundancy of critical components.

### Deny application execution by default

Implement default-deny technologies (such as AppLocker) to only permit applications on an allow-list to execute on the product.

> An allow-list of acceptable applications should be established by the vendor based on the use-cases of the application.

Applies to: Vendor provided hardware
