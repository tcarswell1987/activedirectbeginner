<h2>Active Directory & PowerShell</h2>

<b>Summary:</b> This is a small project with my first experience creating a small business domain with Active Directory using a VM.
After installing OracleVM and downloading .iso files for Windows Server 2019 and Windows 10, I mounted the images to the VM and installed them.
This is the step-by-step process that was used in the creation of the domain.

Open Windows Server 2019, edit the NIC settings to identify the External & Internal NICs, and assign an IP address to the internal network.

<div align="center"<img src="https://imgur.com/9mNLq0i.png" height="400" width="600"></div>

<div align="center><img src="https://imgur.com/3kYvRRr.png" height="400" width="400" class="center"></div>

Proceed to install Active Directory Domain Services onto the Server.

<div align="center"><img src="https://imgur.com/feLPUFM.png" height="400" width="600></div>

<div align="center"><img src="https://imgur.com/UKJrndH.png"></div>

Performed the Post Deployment and named the Domain <b>"mygitproject.com"</b>.

<div align="center"><img src="https://imgur.com/nJUJgVb.png"></div>

Created a new Organizational Unit called <b>"ADMINS"</b>, and created a new user to assign to the ADMINS group.

<div align="center"><img src="https://imgur.com/8KtMxJS.png"></div>

Signed out of the default account, and signed into the account created as a user and admin.

<div align="center"><img src="https://imgur.com/PC7gR2p.png"></div>

Once logged in, install the Remote Access to enable the NAT so that the Client can access the Server and have access to the internet once it's installed.

<div align="center"><img src="https://imgur.com/HMHS0wo.png">

<img src="https://imgur.com/iBVXpjA.png"></div>

Proceeded to set up the DHCP server role on the Server side; added the IP address ranges for Client access.

<div align="center"><img src="https://imgur.com/9t4wcIV.png"></div>

Created the IP address scope through the DHCP Server.

<div align="center"><img src="https://imgur.com/DlOzcbJ.png">

<img src="https://imgur.com/40rW5N1.png">

<img src="https://imgur.com/HXtfum7.png"></div>

Created additional users in the domain; ran the PowerShell automation script to add employees for the Client side.

<div align="center"><img src="https://imgur.com/Uarfi4X.png"></div>

Verified users were created in Active Directory.

<div align="center"><img src="https://imgur.com/Aq53Qc7.png"></div>

Installed Windows 10 VM, logged in and verified internet connectivity, then joined the Client Machine to the domain.

<div align="center"><img src="https://imgur.com/0b2IiBy.png"></div>

Tested the sign-on features for a user on the domain, and verified that the machine recognizes the user.

<div align="center"><img src="https://imgur.com/kPnTvDx.png">

<img src="https://imgur.com/PP8w60c.png"></div>
