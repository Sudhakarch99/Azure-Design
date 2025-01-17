## Overview

This is my Azure Icon Design project for Visio, I aim to maintain this project and provide icon updates as soon new service offerings are available in Azure. I am now maintaining just the 1 version of the stencil as it was too much effort to provide a no-shadow version that inherits the text theme from your drawing. 
<br></br>
Current version (With Shadow and Fixed dark Blue Text) = https://github.com/David-Summers/Azure-Design/blob/master/ICONS_Azure-Full-Colour_V-1.6.vssx
<br></br>
Current Icon set in Picture format (With Shadow and Fixed dark Blue Text)
<br></br>
![Picture](https://github.com/David-Summers/Azure-Design/blob/master/ICONS_Azure-Full-Colour_V-1.6.png)
<br></br>
## Motivation

As far as I know this complete set of Azure Icons in Visio format does not exist, I decided to build a standard set of icons that could be used easily in Design and As-Built diagrams. PowerShell has been used for the conversion process, essentially importing an SVG image into an XML variable and then converting it into Visio Stencil XML format. Most of the icons are based on the publicly available Azure portal icons and some have been drawn by hand as they do not exist.

## Installation

Save the Stencil to your "..\Documents\My Shapes" directory for use within Visio.

## Work in Progress

Design drawing resources, such as Lines\Arrows\Boxes
<br></br>
Blue, Grey and white shaded Visio stencil versions as per the SVG and PNG Icons, I can re-colour every icon into any colour I like using PowerShell so if you would like a customised pallet then let me know and supply the desired colour range in Hex format for example:-
<UL type="Circle">
  <li>
 Maintenance Configuration    Light Blue  = #008dff
  </li>
  <li>
    Azure Blockchain Service
  </li>
  <li>
    Azure Active Directory Identity Secure Score
  </li>
  </ul>
Added a new thing to the list which I might need help with, I want to add search metadata to each icon but cannot figure out how to do it with PowerShell, if you add a search term to an icon it gets written to the Master stencil and not the stencil object. I am currently using "New-Object -ComObject Visio.Application" for scripted interaction.

## Revision History

<B>Current</B>
<br></br>
Version 1.6 - 8/10/2019 - https://github.com/David-Summers/Azure-Design/blob/master/ICONS_Azure-Full-Colour_V-1.6.vssx
<br></br>
Corrected mis-coloured icons, thanks to Cédric De Loor for pointing that out 
<br></br>
Added new icons
<OL type="Circle">
  <li>
  Maintenance Configuration
  </li>
  <li>
  Azure Blockchain Service
  </li>
  <li>
  Azure Active Directory Identity Secure Score
  </li>
  <li>
  Cloud Simple Service
  </li>
    <li>
  Cloud Simple Node
  </li>
    <li>
  Cloud Simple Virtual Machine
  </li>
    <li>
  Azure Lighthouse Service Provider
  </li>
    <li>
  Peering
  </li>
    <li>
  Role
  </li>
    <li>
  Virtual Cluster
  </li>
    <li>
  Azure Active Directory Risk Detection
  </li>  
    <li>
  Azure Active Directory Risky User
  </li>
    <li>
  Azure Active Directory Identity Protection
  </li>
    <li>
  Private Link
  </li>
</ol>
<br></br>
<B><I>Previous</I></B>
<br></br>
Version 1.5 - 26/08/2019 - https://github.com/David-Summers/Azure-Design/blob/master/ICONS_Azure-Full-Colour_V-1.5.vssx
<br></br>
Major change with this release, initially I hand placed the four connection points for each icon and that was not perfect placement. I thought it would be easy to script modify the connection point position (like I did with the Text field in V-1.1) but it turns out that visio does not name a connection point when you add it so I could not modify it through powershell. I added a new script process that allowed me to hand place the connection points and then name them 1-5 (I added a new connection point under the text field for easier south connections when there is data in the text field). Now that they are named, I can modify them when I build my stencil using my gold master. Example below:-
<br></br>
"$shape.CellsU("Connections.1.X").Formula = "Width*0.5""
"$shape.CellsU("Connections.1.Y").Formula = "Height*1.1""
"$shape.CellsU("Connections.2.X").Formula = "Width*-0.1""
"$shape.CellsU("Connections.2.Y").Formula = "Height*0.5""
"$shape.CellsU("Connections.3.X").Formula = "Width*1.1""
"$shape.CellsU("Connections.3.Y").Formula = "Height*0.5""
"$shape.CellsU("Connections.4.X").Formula = "Width*0.5""
"$shape.CellsU("Connections.4.Y").Formula = "Height*-0.05""
"$shape.CellsU("Connections.5.X").Formula = "Width*0.5""
"$shape.CellsU("Connections.5.Y").Formula = "Height*-0.6""
<br></br>
Added new icons
<UL type="Circle">
  <li>
  Dedicated Host
  </li>
  <li>
  Dedicated Host Group
  </li>
  <li>
  Azure Artifact
  </li>
  <li>
  Azure Board
  </li>
</ul>
<br></br>
Version 1.4 - 16/08/2019 - https://github.com/David-Summers/Azure-Design/blob/master/ICONS_Azure-Full-Colour_V-1.4.vssx
<br></br>
Started on the drawing resources, added a colour pallet for what I believe are the best mainly used colours in the stencil range. For fun I scripted an export of every Hex colour value that is being used and there are 88 total colours. Some are extremely close to each other so I selected the most common used colours and included them in the pallet. Added 3 connector styles and deciding on the remaining set. Ideas welcome! and lastly, re-worked the colour scheme on the Azure lighthouse icons.
<br></br>
Added new icons
<UL type="Circle">
  <li>
  SAP Hana
  </li>
  <li>
  Virtual Machine Image Classic
  </li>
  <li>
  Virtual Machine Image Version
  </li>
  <li>
  Virtual Machine Image Definition
  </li>
  <li>
  Virtual Machine Classic
  </li>
  <li>
  Quickstart Center
  </li>
  <li>
  Free Services
  </li>
  <li>
  Help and Support
  </li>
  <li>
  Recent
  </li>
</ul>
<br></br>
<br></br>
Version 1.3 - 14/08/2019 - https://github.com/David-Summers/Azure-Design/blob/master/ICONS_Azure-Full-Colour_V-1.3.vssx
<br></br>
Added new Icons for storage account sub services, had to hand draw these as they did not appear to exist. Renamed Data brick to the correct name Databricks.
<UL type="Circle">
  <li>
  Azure Storage Blob
  </li>
  <li>
  Azure Storage Queue
  </li>
  <li>
  Azure Storage Table
  </li>
  </ul>    
<br></br>
<br></br>
Version 1.2 - 03/08/2019 - https://github.com/David-Summers/Azure-Design/blob/master/ICONS_Azure-Full-Colour_V-1.2.vssx
<br></br>
Removed "Azure" prefix for some incorrectly named icons. 
<br></br>
Added new Icons
<UL type="Circle">
  <li>
  Azure LightHouse Projection
  </li>
  <li>
  Azure LightHouse Management
  </li>
  <li>
  Azure LightHouse Protection
  </li>
  <li>
  Azure LightHouse RBAC
  </li>
  <li>
  Azure Batch
  </li>
  <li>
  Azure Batch Accounts
  </li>
  </ul>    
<br></br>
Version 1.1 - 27/07/2019 - https://github.com/David-Summers/Azure-Design/blob/master/ICONS_Azure-Full-Colour_V-1.1.vssx
<br></br>
First major change, I realised that some of the text fields were not perfectly aligned so I rebuilt my PowerShell process to use dynamic  values for the text field. Since the shapes differ in Height\Width my initial placement was slightly off due to distance from center. This placement is now relative to the bottom edge of the icon. I also inserted the name of the icon into the Text field for page drop as well and reformatted the text to a dark Blue. Final change was to add a subtle drop shadow to each icon as I feel they jump off the page with a small amount of depth. 
<br></br>
Version 1.0 - 25/07/2019 - https://github.com/David-Summers/Azure-Design/blob/master/ICONS_Azure-Full-Colour_V-1.0.vssx
<br></br>
Initial release of the stencil and bonus SVG and PNG versions. I built a conversion process that can re-colour each icon and these initial versions were made with a Blue and Grey scale pallet. 


## Contributors

For requests, issues, idea sharing or just a quick G'Day please use the contact details below.
<br></br>
David Summers - Author - https://twitter.com/Xeeva_D3  

## License

I created these icons while working at www.data3.com.au and we decided to release them to the public for free usage. We felt this was a great community contribution so why keep this to ourselves. My only ask is that you create awesome diagrams and appreciate the effort that I have put into making these. I would love to see some great examples of the icons in use, so Test-Netconnection (Modern way of saying Ping) me on Twitter.
