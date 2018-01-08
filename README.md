# ath10k-firmware
Firmware for Qualcomm Atheros QCA6174 802.11ac [168c:003e] for Dell Precision 5520 Laptop.

## Installation

- Create a backup of your old firmwares

	`sudo cp -R /lib/firmware/ath10k/QCA6174 ~/old_firmware_QCA6174`
	
- Remove old firmware

	`sudo rm -rf /lib/firmware/ath10k/QCA6174`

- Retrieve new firmware

	`git clone http://github.com/afdaniele/ath10k-firmware.git ~/new_firmware_ath10k`

- Copy new firmware

	`sudo  cp -R ~/new_firmware_ath10k/QCA6174 /lib/firmware/ath10k/`

- Reboot

	`sudo shutdown -r now`
