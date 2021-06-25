# kali-linux-random-freeze
kali linux freezes randomly in HP laptops powered by Intel processors.
**This Problem of freezing after some times is noticeswd on Kali linux Dual-boot** 
I have tried all the possible options to get rid of it.
Reinstalled many times and then found a solution i want to share with you.
.
.
.
.
.
.
MY name is anyflick if you like ping my instagram account https://instagram.com/anyflick


.

.
.
.Lets get to the point

after installing Kali linux dual-boot run 
sudo apt-get update && apt-get upgade -y
sudo apt-get dist-upgrade 

cd /etc/defaults
sudo apt install nano  ------------------------------> if not installed earlier
nano grub
Now, read thoroughly and get to the
GRUB_CMDLINE_LINUX_DEFAULT="*****"
replace ***** or whatever you get their to "intel_idle.max_cstate=1"

update-grub
shutdown -r now


hope so your problem has been solved yet..

You can thank me at https://instargam.com/anyflick
