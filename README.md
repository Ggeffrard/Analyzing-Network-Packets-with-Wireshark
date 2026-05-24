# Analyzing-Network-Packets-with-Wireshark
This project demonstrates how to capture and analyze network traffic using Wireshark during a simulated security investigation.

## Technologies Used
- Wireshark
- Windows 10
- Network Traffic Analysis

## Operating Systems Used
- Windows 10

# Explore data with Wireshark

### Step 1: To open the packet capture file, double-click the sample file on the Windows desktop. This will start Wireshark.
<img width="680" height="765" alt="Screenshot 2026-05-13 132159" src="https://github.com/user-attachments/assets/ebd36a54-d0bb-407c-a4d1-e61fc19c1bdc" />

### Step 2: Scroll down the packet list until a packet is listed where the info column starts with the words 'Echo (ping) request'.
<img width="973" height="515" alt="Screenshot 2026-05-13 132701" src="https://github.com/user-attachments/assets/36555714-a011-4366-89e6-985d72ee7b23" />


# Apply a basic Wireshark filter and inspect a packet

### Step 1: Enter the following filter for traffic associated with a specific IP address. Enter this into the Apply a display filter... text box immediately above the list of packets: ip.addr == 142.250.1.139
<img width="973" height="563" alt="Screenshot 2026-05-13 132833" src="https://github.com/user-attachments/assets/d74c4298-2dda-430e-ad57-015f5ab5cb2b" />

### Step 2: Press ENTER or click the Apply display filter icon in the filter text box.
<img width="956" height="686" alt="Screenshot 2026-05-13 132847" src="https://github.com/user-attachments/assets/0c7d4f6d-e179-4cfa-9918-e4caf1e51eab" />

### Step 3: Double-click the first packet that lists TCP as the protocol.
<img width="779" height="754" alt="Screenshot 2026-05-13 132956" src="https://github.com/user-attachments/assets/18024575-897b-4a6a-b1ef-2d9f6e91f101" />

### Step 4: Double-click the first subtree in the upper section. This starts with the word Frame.
<img width="777" height="753" alt="Screenshot 2026-05-13 133056" src="https://github.com/user-attachments/assets/77bb4725-3610-4a06-9595-18a68aeb4399" />

### Step 5: Double-click Frame again to collapse the subtree and then double-click the Ethernet II subtree.
<img width="777" height="747" alt="Screenshot 2026-05-13 133203" src="https://github.com/user-attachments/assets/991f1f6e-3357-4b6d-859a-307a057c48cb" />

<img width="779" height="750" alt="Screenshot 2026-05-13 133304" src="https://github.com/user-attachments/assets/0f4c9df9-49c8-458c-b95b-49c1abb3014f" />

### Step 6: Double-click Ethernet II again to collapse that subtree and then double-click the Internet Protocol Version 4 subtree.
<img width="779" height="747" alt="Screenshot 2026-05-13 133339" src="https://github.com/user-attachments/assets/4f75dd04-f9e9-4609-b59b-2a5a262c5218" />

<img width="776" height="747" alt="Screenshot 2026-05-13 133411" src="https://github.com/user-attachments/assets/879569a9-643b-48d8-84e1-c0d2ee10e55b" />

### Step 7: Double-click Internet Protocol Version 4 again to collapse that subtree and then double-click the Transmission Control Protocol subtree.
<img width="781" height="749" alt="Screenshot 2026-05-13 133519" src="https://github.com/user-attachments/assets/126b0767-aa2b-44bb-a835-4cdefd8341da" />

<img width="777" height="750" alt="Screenshot 2026-05-13 133604" src="https://github.com/user-attachments/assets/eb5dcbcd-1d45-4df5-861e-5fcf6593b25e" />

### Step 8: In the Transmission Control Protocol subtree, scroll down and double-click Flags.
<img width="774" height="746" alt="Screenshot 2026-05-13 133741" src="https://github.com/user-attachments/assets/b2e5aa7b-41a8-41a8-ac7d-bae590d2fc48" />

### Step 9: Click the X icon to close the detailed packet inspection window.
<img width="788" height="737" alt="Screenshot 2026-05-13 133829" src="https://github.com/user-attachments/assets/fcdd9a9f-3fdc-4904-8990-fc5a677535be" />

### Step 10: Click the X Clear display filter icon in the Wireshark filter bar to clear the IP address filter.

<img width="892" height="516" alt="Screenshot 2026-05-13 133907" src="https://github.com/user-attachments/assets/1ef27f5c-2fcb-4e07-96f9-098034766c9f" />

# Use filters to select packets

###  Step 1: Enter the following filter to select traffic for a specific source IP address only. Enter this into the Apply a display filter... text box immediately above the list of packets: ip.src == 142.250.1.139
<img width="1861" height="917" alt="Screenshot 2026-05-24 161425" src="https://github.com/user-attachments/assets/b867e8c2-2955-4859-b964-102ed36e971e" />

###  Step 2: Press ENTER or click the Apply display filter icon in the filter text box.
<img width="1916" height="415" alt="Screenshot 2026-05-24 161634" src="https://github.com/user-attachments/assets/10e0ad08-00d2-406e-92cb-e49ef4d0a72b" />
A filtered list is returned with fewer entries than before. It contains only packets that came from 142.250.1.139.

### Step 3: Click the X Clear display filter icon in the Wireshark filter bar to clear the IP address filter.
<img width="1909" height="477" alt="Screenshot 2026-05-24 161955" src="https://github.com/user-attachments/assets/e77c52b8-b95b-4f68-b2ff-bac69711a3d1" />

### Step 4: Enter the following filter to select traffic for a specific destination IP address only: ip.dst == 142.250.1.139
<img width="1917" height="784" alt="Screenshot 2026-05-24 162040" src="https://github.com/user-attachments/assets/84e070fe-33e9-4187-826a-1699a2398ec4" />

### Step 5: Press ENTER or click the Apply display filter icon in the filter text box.
<img width="1915" height="777" alt="Screenshot 2026-05-24 162056" src="https://github.com/user-attachments/assets/78412a49-4453-435c-b00b-bde94f8b1c2b" />
A filtered list is returned that contains only packets that were sent to 142.250.1.139.

### Step 6: Click the X Clear display filter icon in the Wireshark filter bar to clear the IP address filter.
<img width="1914" height="632" alt="Screenshot 2026-05-24 162851" src="https://github.com/user-attachments/assets/807b0902-1086-46d3-9746-273294e39f5d" />

### Step 7: Enter the following filter to select traffic to or from a specific Ethernet MAC address. This filters traffic related to one MAC address, regardless of the other protocols involved: eth.addr == 42:01:ac:15:e0:02
<img width="1915" height="801" alt="Screenshot 2026-05-24 163129" src="https://github.com/user-attachments/assets/45784b6a-2b10-4421-ab62-a15da7c68f7e" />

### Step 8: Press ENTER or click the Apply display filter icon in the filter text box. Double-click the first packet in the list. You may need to scroll back to display the first packet in the filtered list.
<img width="1581" height="665" alt="Screenshot 2026-05-24 163718" src="https://github.com/user-attachments/assets/d0b3776c-a064-4a86-88dc-12548e5db352" />
<img width="1531" height="755" alt="Screenshot 2026-05-24 163754" src="https://github.com/user-attachments/assets/63db9c1b-d18c-47b1-b757-9eb0820e5fca" />

### Step 9: Double-click the Ethernet II subtree if it is not already open.
<img width="1534" height="745" alt="Screenshot 2026-05-24 163854" src="https://github.com/user-attachments/assets/24f1f3e0-e60c-44b2-99db-cd3d01faa720" />

### Step 10: Double-click the Ethernet II subtree to close it. Double-click the Internet Protocol Version 4 subtree to expand it and scroll down until the Time to Live and Protocol fields appear.
<img width="1534" height="749" alt="Screenshot 2026-05-24 164012" src="https://github.com/user-attachments/assets/c27cd6fb-48f2-43de-b998-2c2df86f4df1" />
<img width="1535" height="750" alt="Screenshot 2026-05-24 164123" src="https://github.com/user-attachments/assets/1eca4329-a1c0-43a6-b59e-bb4f0f0069c5" />
<img width="1512" height="215" alt="Screenshot 2026-05-24 164207" src="https://github.com/user-attachments/assets/57550330-ff7a-425d-8f0d-817d415c4672" />

Step 11: Click the X icon to close the detailed packet inspection window.
<img width="1540" height="751" alt="Screenshot 2026-05-24 164306" src="https://github.com/user-attachments/assets/94857aa9-64e4-4966-81fa-67b7c1789f82" />

Step 12: Click the X Clear display filter icon in the Wireshark filter bar to clear the MAC address filter.
<img width="1862" height="718" alt="Screenshot 2026-05-24 164404" src="https://github.com/user-attachments/assets/2a37ba61-bcb9-43a8-a76b-cd677869d8f3" />




