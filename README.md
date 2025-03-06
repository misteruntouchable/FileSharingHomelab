# FileSharingHomelab

 ### [Pictoral Walkthrough Demonstration]

<h2>Prerequisites</h2>
   For this lab we will not get into how to install virtual box or Active Directory. Oracle Box should be downloaded and installed, Windows Server 19 
   should have been downloaded and installed. Windows 10 Pro should have been installed for your client VM; Active Directory Domain Services should be 
     installed and configured.  And Group Policy Managment Console must also be installed on your Windows Server.
 

 <h2>Description</h2>
  In this lab we are going to set up File Services and File Sharing within Active Directory. We will create File sharing on a Windows Server and we will discuss
  what is Network Sharing, Permission Types, and how to implement File Service Resource Manager. So File and Folder Sharing is the practice of making all these
  resources available for memebers within your company to make edits, sharing and  modifying of files easier. There are two types of Network Sharing a)Local and 
  b) Network. There are also different types of Permission and Access Control ie; Read, Write, Full Control, and Execute. Third, we have two types of Permissions
  a) NTFS and b) Share. And finally, we have two types of Sharing Methods which are a)Mapped and b)Network

  
  <h2>Program walk-through:</h2>
  
<p align="center">
    The differences between a Shared Permisson and a NTFS Permission.
     Here is the SHARED Permission <br/>
 <img src="https://imgur.com/EabOV0E.png" height="80%" width="80%" "/>
<p align="center"> For Shared Permissions there are only three options. Also in the Shared Permissions you can set the permissions on the folder level only. 
                   It is not applied to the sub-folders or files under it.</br>
   
</br>

</br>                   
</br>

<p align="center">
    The NTFS Permission <br/>
 <img src="https://imgur.com/XwtqDov.png" height="10%" width="30%" "/>
<p align="center"> In NTFS one of the obvious main differences with that NTFS has more permissions. In NFTS you can apply permissions to the files and  
                   folder level. Permissions can be also applied to sub-folders here.</br>
   
</br>

</br>                   
</br>
<p align="center">
    Let's begin with Setting Up a File Sharing <br/>
 <img src="https://imgur.com/ANCJ8WX.png" height="60%" width="60%" "/>
<p align="center">In this task we are going to configure file sharing by create shared folders first so we have can have something to share. We will give it 
                  appropriate permissions. Then we are going to set NTFS and share permissions to allow domain users access to it. Go to the Windows Server and 
                   login. Then open up file explorer, we want to create a folder to share later. Click on the Local Disk and create and ordinary folder. We can 
                   call it SHARED. Once you have created the folder you can right click on it and go to properties. Here we want to set of Shared 
                   Permissions. This will be the general permission access which will apply at the folder level. If you want more detailed access for 
                   for particular folders, sub-folders, or files you can do NTFS permissions. So next, in the properties box, hit the Sharing tab then click on 
                    advanced sharing. </br>
   
</br>

</br>                   
</br>

<p align="center">
    Advanced Sharing <br/>
 <img src="https://imgur.com/LaXfFMo.png" height="60%" width="60%" "/>
<p align="center"> In Advanced Sharing we want to check share this folder , becuase we want it to share over the network. And you hit the Permissions 
                   you will be able grant permission for Domain Users. It will able accessible to everyone under the domain. So to add folder within a domain 
                   click add then search for the domain you want to add the folder to and apply. And for the confguration of the folder itself, you can choose 
                   which of the three options you want the users to have the capacity to have with the folder; read, change or full control. Then ok and 
                   apply.</br>
   
</br>

</br>                   
</br>

<p align="center">
    For the NTFS Permissions<br/>
 <img src="https://imgur.com/upNnSs7.png" height="60%" width="60%" "/>
<p align="center"> To get to the NTFS permissions, hit the security tab in the Shared Properties Box. Here, you have the ability to do alot more permissions.
                   Here, will also see a lot more groups or user names. You have the ability here to give permission to groups or just one individual user in 
                   NTFS. So after we have made our configurations we will have an shared folder.</br>
   


</br>                   
</br>

<p align="center">
    The Next task we want to do is set up our Client Machine to access the Shared Resource we have created<br/>
 <img src="https://imgur.com/upNnSs7.png" height="60%" width="60%" "/>
<p align="center"></br>
   


</br>                   
</br>


