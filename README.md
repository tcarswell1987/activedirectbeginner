<h2>Active Directory For A Beginner & PowerShell</h2>

This is a small project with my first experience creating a small business domain with Active Directory using a VM.
After installing OracleVM and downloading .iso files for Windows Server 2019 and Windows 10, I mounted the images to the VM and installed them.

Beginning with Windows Server 2019, I edited the NIC settings to identify the external & internal NICs and assigned the IP.

<div align="center"<img src="https://imgur.com/9mNLq0i.png" height="400" width="600"></div>

<div align="center><img src="https://imgur.com/3kYvRRr.png" height="400" width="400" class="center"></div>

I then proceeded to install Active Directory Domain Services onto the Server.

<div align="center"><img src="https://imgur.com/feLPUFM.png" height="400" width="600></div>

<div align="center"><img src="https://imgur.com/UKJrndH.png"></div>

Performed the Post Deployment and named the Domain <b>"mygitproject.com"</b>.

<div align="center"><img src="https://imgur.com/nJUJgVb.png"></div>

Created a new Organizational Unit called <b>"ADMINS"</b>, and created myself as a new user to assign into the ADMINS group.

<div align="center"><img src="https://imgur.com/8KtMxJS.png"></div>

Signed out of the default account, and signed into the account created for myself as a user and admin.

<div align="center"><img src="https://imgur.com/PC7gR2p.png"></div>

Once logged in, I installed the Remote Access to enable the NAT so that the client will be able to access the server and internet access once it's installed.

<div align="center"><img src="https://imgur.com/HMHS0wo.png">

<img src="https://imgur.com/iBVXpjA.png"></div>

Proceeded to set up the DHCP server role on the server side; added IP address ranges for client access.

<div align="center"><img src="https://imgur.com/9t4wcIV.png"></div>

Created IP address scope through the DHCP Server.

<div align="center"><img src="https://imgur.com/DlOzcbJ.png">

<img src="https://imgur.com/40rW5N1.png">

<img src="https://imgur.com/HXtfum7.png"></div>

To create additional users in the domain, I ran a PowerShell script to add mock employees for the client side.

<div align="center"><img src="https://imgur.com/Uarfi4X.png"></div>

Verified users were created in Active Directory.

<div align="center"><img src="https://imgur.com/Aq53Qc7.png"></div>

After installing the Windows 10 VM, I proceeded to log in, verify internet connectivity, and join the Client Machine to the domain.

<div align="center"><img src="https://imgur.com/0b2IiBy.png"></div>

Afterwards, I tested the sign-on features for one of the "employees" on the domain, and verified that the machine recognizes the user.

<div align="center"><img src="https://imgur.com/kPnTvDx.png">

<img src="https://imgur.com/PP8w60c.png"></div>
