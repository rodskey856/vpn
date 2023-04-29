<p align="center">
<img src="https://i.imgur.com/QurLqjG.png" height="40%" width="60%"/>
</p>

<h1>Observing the Effect of a VPN on IP Addressing</h1>
In this project, I observed the impact of a virtual private network (VPN) on IP address, location, and web browsing. <br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
-	Remote Desktop
-	ProtonVPN (free version)


<h2>Operating System Used </h2>

- Windows 10 (21H2)

<h2>High-Level Steps</h2>

-	Create a Windows 10 virtual machine in Azure
-	Remote Desktop into the virtual machine
-	Use whatismyipaddress.com to find the IP address and location for the VM
-	Download the free version of ProtonVPN (create an account if there is no preexisting account)
-	In ProtonVPN, connect to a server in another country
-	Use whatismyipaddress.com to find the new IP address and location for the VM
-	Browse a webpage to see if there are any changes to the URL or language
-	Delete Resource Groups in Azure


<h2>Synopsis</h2>

<br />

<p>
<img src="https://i.imgur.com/JkqLm3d.png" height="70%" width="70%"/>
</p>
<p>
I went on the Azure Portal. Created a Virtual Machine with the location of Japan, East. Opened the IP address in Remote Desktop.
</p>
<br />

<p>
<img src="https://i.imgur.com/mJnKiLg.png" height="70%" width="70%"/>
</p>
<p>
I opened up the Microsoft Edge. In the address bar, entered "whatsmyipaddress.com". This website will display the IP location and IP address. This is my first location. (Tokyo, Japan) Now that we know the IP address and location of the VM, let’s see how it changes when using a VPN! 
</p>
<br />

<p>
<img src="https://i.imgur.com/tTDHtde.png" height="70%" width="70%"/>
</p>
<p>
I had previously created a free ProtonVPN account in order to do this lab, so now I just logged into my account and downloaded ProtonVPN.
</p>
<br />

<p>
<img src="https://i.imgur.com/eRdbWXt.png" height="70%" width="70%"/>
</p>
<p>

</p>
</p>
<br />

<p>
<img src="https://i.imgur.com/7af61VN.png" height="70%" width="70%"/>
</p>
<p>
I selected a server in Netherlands, then noticed the changes in ProtonVPN. One of the significant changes was that my IP address in the VPN was now different from the VM’s IP address (compare the IP address in the top left corner of my screen to the IP address in the top left corner of the VPN).
</p>
<br />
                                                                   
<p>
<img src="https://i.imgur.com/q9anpdq.png" height="70%" width="70%"/>
</p>
<p>
I still had whatismyipaddress.com open in the Edge browser, so I simply refreshed the page to view any changes. According to the website, my IP address was now the one shown in the VPN, and my location was Tokyo, Japan! This is because my physical computer was connected to the VM, which was now connected to a VPN server in Netherlands.
</p>                                                                   
<p>
<img src="https://i.imgur.com/OVfJ0SL.png" height="70%" width="70%"/>
</p>
<p>                                                                               
As we can see, when I searched the term “amazon” using Google, the search results were in Japanese. This further confirmed that the VPN worked.
</p>

<br />
