# File Permission Lab

<h2>Project description</h2>
As an active participant in my Google Cybersecurity course, I successfully encountered file permissions in the projects directory, and reinforced system security. Through careful assessment and utilization of commands like “ls -la” and “chmod”, I effectively adjusted authorization levels to protect critical files and directories. My proficiency in Linux file permissions management, demonstrated through meticulous documentation, thorough checks, and practical implementation, highlights my commitment to continuous learning and my ability to mitigate risks in organizational settings. 
<br />

<h2>Coding Language</h2>

- <b>Linux</b>


<p align="center">
<h2>Check file and directory</h2>
The following code demonstrates how I used Linux commands to determine the existing permissions set for a specific directory in the file system. 

<img src="https://i.imgur.com/Pg7z3G4.png" height="70%" width="70%" alt="Disk Sanitiation Step"/>

In the lab, I executed the “ls -la” command to obtain a detailed listing of the files in the projects directory, including hidden files. The resulting output displayed one directory named “drafts”, one hidden file named “.project_x.txt,” and five other project files. The 10-character string in the first column represents the permissions assigned to each file or directory. This exercise allowed me to gain insight into the existing permissions structure and better understand the access rights associated with the files within the projects directory. 

<h2>Describe the permission string</h2>
The 10-character string associated with file permissions can be analyzed to determine the authorized users and their specific access  rights. Here’s a breakdown of the characters and their  meanings:


* The 1st character represents the file type, where “d” indicates a directory and “-” denotes a regular file. 

* The 2nd-4th character indicates the user’s read ( r ), write ( w ), and executed ( x ) permissions. A hyphen (-) signifies the absence of the permission.

* The 5th-7th characters indicated the group’s read, write and execute permissions. A hyphen (-) indicates the lack of a specific permission. 

* The 8th-10th characters represent the permissions for other, referring to all users except the owner and the group. A hyphen (-) indicates the absence of a particular permission. 

For instance, in the example of “project_t.txt ’’ with the permission string “-rw-rw-r- -,” the file is identified as a regular file (not a directory). The user, group and others have read permissions ( r ) in the 2nd, 5th and 8th positions. The user and group also have write permissions (w) in the 3rd and 6th positions. However, no one has execute permissions for “project_t.txt.” 
<br />


<p align="center">
<h2>Change file permission</h2>
As part of my lab, I successfully completed a lab focused on securing files. I addressed the organization’s directive to restrict write access for “other” users. By analyzing the file permissions I had previously obtained, I identified “project_k.txt” as requiring modifications. Taking appropriate action, I removed the write access for “other” on the file, effectively enforcing the organization’s security policy.

The following code demonstrates how I used Linux command to do this:

<img src="https://i.imgur.com/eYTvaTn.png" height="70%" width="70%" alt="Disk Sanitiation Step"/>

In the provided screenshot, the first two lines showcase the commands executed, while the subsequent line illustrates the output of the second command. The “chmod” command was used to modify the file and directory permissions. The first argument denotes the permissions to be changed, while the second argument specifies the target file or directory. In this particular instance, I successfully removed the write permission from other for the “project_k.txt” file. After this, I used “ls -la” to review the update I made. 
<br />


<P align="center">
<h2>Change file permission on a hidden file</h2>
I actively engaged in a lab exercise where I focused on securing critical files. As part of the lab, I successfully implemented measures to protect the “project_x.txt” file, preventing unauthorized write access. By carefully managing permissions, I ensured that only the designated user and group retained read access, aligning with the principles of secure file management taught in the course. 

The following code demonstrates how I used Linux commands to change the permissions:

<img src="https://i.imgur.com/jr5Vl7R.png" height="70%" width="70%" alt="Disk Sanitiation Step"/>

The screenshot captures the sequence of commands I executed, along with their corresponding outputs. By recognizing that “.project_x.txt” is a hidden file denoted by the preceding period, I proceeded to modify its permissions. Specifically, I revoked write permission for both the user and group, while granting read permissions exclusively to the group. To achieve this, I utilized the commands “u-w” to remove write permissions for the user, “g-w” to remove write permissions for the group, and “g+r” to add read permissions for the group. 
<br />


<p align="center">
<h2>Change directory permissions</h2>
I successfully enforced access control measures for the drafts directory, in accordance with my organization’s security requirements. Specifically, I restricted execute permissions to only the reseacher2 user, thereby preventing unauthorized access. By implementing these measures, I demonstrated my proficiency in access control to cybersecurity best practices.

The following code demonstrates how I used Linux commands to change the permissions:

<img src="https://i.imgur.com/SDd0juW.png" height="70%" width="70%" alt="Disk Sanitiation Step"/>

I showcased the commands I executed and their corresponding output. Recognizing that the group had unnecessary execute permissions, I utilized the “chmod” command to revoke them. As for the reseacher2  user, who already possessed the required execute permissions, no further adjustments were necessary. 
<br />

<p align="center">
<h2>Summary</h2>
I successfully adjusted multiple file and directory permissions to meet the specified authorization level dictated by the exercise. The  initial step involved examining the permissions of the projects directory using the “ls -la” command, allowing me to make informed decisions. Subsequently, I employed the “chmod” command iteratively to modify permissions, ensuring strict adherence to the desired security requirements. This hand-on experience demonstrated my practical understanding of permission management and its significance in maintaining a secure computing environment.
<br />






