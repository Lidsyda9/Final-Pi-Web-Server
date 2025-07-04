<!-- markdownlint-configure-file { "MD004": { "style": "consistent" } } -->
<!-- markdownlint-disable MD033 -->
#

<p align="center">
<img src="https://upload.wikimedia.org/wikipedia/en/thumb/c/cb/Raspberry_Pi_Logo.svg/512px-Raspberry_Pi_Logo.svg.png" 
     alt="Raspberry Pi Logo" width="168" height="270">
  <br>
  <strong>Homework source code and guide how to set up Web Server  https://forums.raspberrypi.com/viewtopic.php?t=24441</strong>
</p>

<!-- markdownlint-enable MD033 -->

# How to Set Up a Web Server on a Raspberry Pi – Host Your Own Website! What You Need. Below is everything you need to set up your Raspberry Pi to become a fully functional personal web server.


- **A Raspberry Pi** Single-Board Computer (in my case I have used a Raspberry Pi Zero W Rev 1.1 Model 512MB)
- First, you’ll need to install Raspberry Pi OS on your Pi.
- Raspberry Pi Zero 2 W
- microSD card (8GB or larger)
- micro USB power supply
- Internet connection (Wi-Fi or Ethernet)
- (Optional) External monitor/keyboard OR SSH access
- Power supply


 # Update Raspberry Pi
 
`sudo apt update && sudo apt upgrade -y`
 
# Install Apache (basic web server)

`sudo apt install apache2 -y`


# Check if it works
Open my Pi's IP address in a browser, type in the provided IP Address followed by | /admin | into the URL of any internet browser. In my case I typed | http://192.168.0.28/ |. Then you should see the **Apache2 Debian Default Page**

# Add Your Own Web Page

`cd /var/www/html`

Replace the Html content with my own message:

`sudo nano index.html`

# My Raspberry Pi Project
This project sets up a simple web server using a Raspberry Pi Zero.
## Website Preview

**`<h1>Hello from My Raspberry Pi Server!</h1>`** and **`<p>This website is powered by a Pi Zero and built as part of my final project.</p>`**

## Features

- Raspberry Pi Zero W as the host
- Static HTML content
- Apache web server
>Running:
>`sudo chown www-data:www-data /var/www/html/index.html`

**Open Web Browser and visit:**

 <strong> set up Web Server  https://<my_pi_ip></strong>

 ![Set up Web server Final project](https://github.com/user-attachments/assets/31850eae-317d-4678-892f-3cbf335075d3)

