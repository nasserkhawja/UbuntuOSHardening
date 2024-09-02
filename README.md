# UbuntuServerHardening

The basics of what it does. Keep in mind this disables root via ssh.

Update the System

Ensures that all software packages are up-to-date with the latest security patches.
Install and Configure a Firewall (UFW)

Installs UFW, a user-friendly firewall. The default policy denies all incoming traffic and allows outgoing traffic, with OpenSSH explicitly allowed.
Disable Unused Services

Disables and stops services like Telnet and FTP that are not needed to reduce the attack surface.
Set Up Fail2ban

Installs Fail2ban to protect against brute-force attacks by banning IPs that have multiple failed login attempts.
Configure Password Policies

Enforces strong password policies by setting maximum and minimum password ages, minimum length, and warning period.
Disable Root Login via SSH

Disables direct root access over SSH to prevent unauthorized access to the root account.
Install and Configure auditd

Installs and configures auditd for auditing system changes, providing logs of sensitive file accesses and modifications.
Enable AppArmor

Ensures AppArmor is enabled and running. AppArmor provides Mandatory Access Control by restricting programs' capabilities with per-program profiles.
Remove Unnecessary Packages

Cleans up unused packages to reduce potential vulnerabilities.
Verify File Permissions

Ensures proper permissions for critical files to protect against unauthorized access.
Important Notes
Customization: Adjust the script according to your specific security requirements and Ubuntu version.
Testing: Always test scripts in a safe environment before applying them to production systems.
Review: Regularly review and update security practices to adapt to new threats.
