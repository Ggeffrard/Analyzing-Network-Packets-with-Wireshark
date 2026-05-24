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








