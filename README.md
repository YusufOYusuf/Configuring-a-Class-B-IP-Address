<h1>Configuring a Class B IP Address</h1>



<h2>Description</h2>
In this lab, I learned to configure a Class B IP address. In a Class B network, the first 16 bits are the network part of the address. All Class B networks have their first bit set to a 1 an dthe second bit set to a 0. There are 16,384 possible Class B networks.
<br />



<h2>Environments Used </h2>

- <b>Windows Server 2016 Standard</b> 


<h2>Languages and Utilities</h2>

- <b>Windows Powershell<b>

<h2>Program walk-through:</h2>

<p align="center">
Right click the start Menu and open Network Connections: <br/>
<img src="https://i.postimg.cc/bvsn0jpk/Screen-Shot-2022-06-23-at-3-15-34-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />
  
  
<br>
In the Network Connections window, double click the Ethernet 2 network adapter:<br>
<img src="https://i.postimg.cc/3xPHB7mf/Screen-Shot-2022-06-25-at-7-22-31-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />
  
  
  
<br />
In the Ethernet 2 status dialog box, click Properties:</br>
<img src="https://i.postimg.cc/ry3XcMYV/Screen-Shot-2022-06-25-at-7-24-01-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />
  
  
  
<br />
In the Ethernet 2 Properties dialog box, under This connection uses the following items double click Internet Protocol Version 4(TCP/IPv4:  <br/>
<img src="https://i.postimg.cc/G3G2Z7q5/Screen-Shot-2022-06-25-at-7-25-17-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />


<br />
IN the Internet Protocol Cersion 4 (TCP/IPv4) Properties dialog box, select Use the following IP address and type in IP address,subnet mask,default gateway,preferred DNS server and alternate DNS Server:  <br/>
<img src="https://i.postimg.cc/MZm5m8h6/Screen-Shot-2022-06-25-at-7-30-31-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />



<br />
Click start menu and open Windows powershell:  <br/>
<img src="https://i.postimg.cc/x1J5YZ4f/Screen-Shot-2022-06-23-at-3-31-44-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />




<br />
In Windows Powershell window execute the following command to get the IP address of the Ethernet network adapter: (Get-NetAdapter -Name "Ethernet 2" | Get-NetIPAddress).IPAddress:  <br/>
<img src="https://i.postimg.cc/SsMSbdbd/Screen-Shot-2022-06-25-at-7-35-19-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />





<br />
You will observe the IP address 135.58.24.17:  <br/>
<img src="https://i.postimg.cc/T13tW72q/Screen-Shot-2022-06-25-at-7-38-05-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />







</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
