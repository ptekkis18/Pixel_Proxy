# Pixel_Proxy
Repurposed laptop to run Pi-Hole for ad and malware blocking

<p align="center">
  <img src="https://github.com/user-attachments/assets/9ceabf4e-5740-44a2-89f2-984499c8f984" width="256" height="256" />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <img src="https://github.com/user-attachments/assets/6af2512a-6d6b-40fc-8ef3-3368728a6703" width="200" height="200" />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <img src="https://github.com/user-attachments/assets/733e6c35-ec6e-4579-8c2f-0b7883d66407" width="158" height="230" />
</p>

# Background Section

Laptop Model: Toshiba Satellite

This laptop was used for everything ranging from document creation for school to light gaming. Initially the battery declining reassuring it useless without being constantly on the charger. Soon after rocket league was released and after acknowledging the laptop was not meeting even the minimum requirements, it was still used to play the game at the lowest possible settings.

After a long gaming session, the laptop automatically turned off. Assuming the problem was the battery, the laptop was left to cool and recharge as seen from the battery indicator colour orange. After being fully charged and cooled, the laptop was turned on only to be greeted with a black screen. 

Upon further inspection, using the VGA socket to output display signal on an external monitor windows blue screen of death keep appearing along with pixel artifacts as seen from the images bellow. This revealed that the integrated graphics card as well as the intel graphics card were damaged from intense heat and prolonged gaming session.
<p align="center">
  <img src="https://github.com/user-attachments/assets/4f5243a7-dc52-4617-a119-37786b9c4845" width="154" height="200" />
</p>

# Goal
Repurpose the laptop and make it as usable as possible


# Alpine Linux
<p align="center">
  <img src="https://github.com/user-attachments/assets/6ff70225-98d9-4984-bb9f-d8d0bea95ea4" width="296" height="200" />
</p>
Firstly, the old hard disk drive was extracted preserving all the important files and replaced with a 4GB USB drive. Then, Linux Alpine was installed and used as the operating system as it is the lightest Linux distro allowing it to run with minimal resources. 

The installation went smoothly despite the fact that the screen hardly could be seen. This was made possible with the way Alpine Linux works allowing for live use of the system just like Kali. Once you advance through the installation and as soon as OpenSSH is executed, the laptop could be access through another machine enabling installation completion.

# Docker
Additionally, docker was installed to enable the use of a portable Pi-Hole. The container was created and run with the configured settings to enable the Pi-Hole to run as intended. Ports were opened and firewall rules had been set to enable the laptop to receive and route DNS request from the main router. 

# Main Router
The DNS settings had been updated to include the laptop's IP address as the primary DNS resolver followed with Cloudflare DNS as a backup option.

# Conclusion
During the execution of this project a lot of challenges were presented, technologies explored and finally the goal was achieved. The installation of Alpine Linux was simple to understand and follow allowing the process to be easily learned along the way without needing to dive into installation guides and Linux commands. Docker and its containers were easily researched and understood with lots of information provided from the community offerings useful resources from installation to custom container configuration for running Pi-Hole.

Lastly, the root cause of the problem. The screen and graphics card made the situation even worse by displaying artifacts and blocking useful parts of the screen. Luckily, even this challenge was overcome with OpenSSH allowing the project to advance and be completed successfully.

Even with the damaged screen output provided from the VGA port when connected to an external monitor, the laptop was successfully repurposed with no additional expenses. The Pi-Hole is operating as intended to this day, blocking and preventing websites from displaying ads and malware maintaining a safe and secure cyber environment with uninterrupted browsing experience for all users in the network.

