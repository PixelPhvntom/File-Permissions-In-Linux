# File Permissions In Linux 🔐

This project showcases my Linux-based file permissions management to enforce organizational security standards. Includes verifying current permissions, analyzing access rights, and applying chmod to control user and group access. Demonstrates expertise in Linux, access control, and security compliance for robust system security.

## Project 

### 1. Checking File and Directory Permissions
   
Using the ls -la command, I reviewed the permissions for files and directories within the projects directory. This command provides a detailed listing, including hidden files, showcasing the 10-character permission string (e.g., -rw-rw-r--), and permissions for the user, group, and others.

   <img width="814" alt="Screenshot 2024-11-07 at 5 08 47 PM" src="https://github.com/user-attachments/assets/068fdcd7-d17a-4fbf-acbc-a650f42a26e2">

### 2. Interpreting Permission Strings
   
The permission string’s structure reveals access levels:

  - First character: Indicates type (d is for directory, - is for file).
  - 2nd-4th characters: Permissions for the user.
  - 5th-7th characters: Permissions for the group.
  - 8th-10th characters: Permissions for others.

    To note: r is for read, w is for write, and x is for execute

    Example: The permissions -rw-rw-r-- for project_t.txt show that the user and group have read and write access, while others have read-only access.

### 3. Modifying Permissions
   
The organization determined that others shouldn't have write access to any of their files. To enforce security policies, I used the chmod o-w project_k.txt command to restrict write access. I subsequently verified the updated permissions using ls -la to ensure compliance with organizational security standards.

   <img width="811" alt="Screenshot 2024-11-07 at 5 32 34 PM" src="https://github.com/user-attachments/assets/d0ad6a84-000c-4383-a626-b7a85b698d87">

### 4. Modifying Permissions
   
The research team recently archived project_x.txt, and write access is no longer required for any users. However, both the user and group should retain read access to this file. To comply with security measures, I used chmod u-w, g-w, g+r .project_x.txt command to removed write access while ensuring read access remains. Following the changes, I executed ls -la to ensure that the permissions met the organization’s security requirements.

   To note: .project_x.txt as a hidden file (indicated by the period)

   <img width="816" alt="Screenshot 2024-11-07 at 5 49 24 PM" src="https://github.com/user-attachments/assets/ba40f6ee-8f92-4d9c-aef8-565fa2ac0bfb">

### 4. Setting Directory Permissions

The organization required only the user to have execute access to the drafts directory. I used chmod g-x drafts to restrict permissions for group, leaving execute permissions solely for the user. To verify compliance with security policies, I reviewed the modified permissions using the ls -la command.

   <img width="813" alt="Screenshot 2024-11-07 at 5 54 28 PM" src="https://github.com/user-attachments/assets/513721f5-0a46-478e-9dc3-a6a9d3dd65fb">

## Summary

I modified permissions across several files and directories to align with the organization's security and access control standards, ensuring secure and compliant Linux-based system management.


## License

MIT. This project is open-source.
