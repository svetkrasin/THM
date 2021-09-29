# DHCP Discover (DHCP starvation attack)

dhcp.option.dhcp == 1

# DHCP Offer

dhcp.option.dhcp == 2

# DHCP Request

dhcp.option.dhcp == 3

# SSID (Human readable wireless network name)

IEEE 802.11 wireless LAN > Tagged parameters > Tag: SSID parameter set > SSID

# BSSID

IEEE 802.11 Beacon frame > BSSID

# Type of wireless security

IEEE 802.11 wireless LAN > TAgged parameters > Tag: Vendor Speccific: WPA Information Element > WPA Version

## For non-WPA

Wireless > Protection

# Decrypt wireless traffic

aircrack-ng PacketName.pcap

wireshark PacketName.pcap

View > Wireless Toolbar > 802.11 > 802.11 preferences > Enable Decryption > Edit > +  > WEP KeyName > OK 
