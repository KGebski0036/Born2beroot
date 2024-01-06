# Born2beroot

This project aims to introduce you to the wonderful world of virtualization and set up own operating system while implementing strict rules.

## Tehnologies

<div align="center">
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" height="30" alt="linux logo"  />
</div>

## Requirements

- Create at least 2 encrypted partitions using LVM.
- A SSH service will be running on port 4242 only.
- It must not be possible to connect using SSH as root.
- Configure your operating system with the UFW firewall and thus leave only port 4242 open.
- The hostname of your virtual machine must be kgebsk42
- Implement a strong password policy.
- Install and configure sudo following strict rules.
- User with kgebski as username has to be present.
- This user has to belong to the user42 and sudo groups.
- Password has to expire every 30 days.
- The minimum number of days allowed before the modification of a password will
be set to 2.
- The user has to receive a warning message 7 days before their password expires.
- Your password must be at least 10 characters long. It must contain an uppercaseletter, a lowercase letter, and a number. Also, it must not contain more than 3consecutive identical characters.
- The password must not include the name of the user.
- The following rule does not apply to the root password: The password must have
at least 7 characters that are not part of the former password.
- Authentication using sudo has to be limited to 3 attempts in the event of an incorrect password.
- A custom message has to be displayed if an error due to a wrong password occurs when using sudo.
- Each action using sudo has to be archived, both inputs and outputs. The log file
has to be saved in the /var/log/sudo/ folder.
- The TTY mode has to be enabled for security reasons.
- For security reasons too, the paths that can be used by sudo must be restricted
- At server startup, the script will display some information (listed below) on all terminals every 10 minutes
1. The architecture of your operating system and its kernel version.
2. The number of physical processors.
3. The number of virtual processors.
4. The current available RAM on your server and its utilization rate as a percentage.
5. The current available memory on your server and its utilization rate as a percentage.
6. The current utilization rate of your processors as a percentage.
7. The date and time of the last reboot.
8. Whether LVM is active or not.
9. The number of active connections.
10. The number of users using the server.
11. The IPv4 address of your server and its MAC (Media Access Control) address.
12. The number of commands executed with the sudo program.
