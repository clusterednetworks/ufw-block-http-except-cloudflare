# ufw-block-http-except-cloudflare
This is a shell script that will allow your to block all http and https traffic
from the internet and allow only cloudflares IP Block. It will then generate a ufw allow command
for all of Cloudflares IP Block.

This script is designed for debian based linux servers using the UFW (Uncomplicated Firewall)

Using this script properly will essentially give your server the best DDoS protection as it
will force all http/https traffic through cloudflare.

# Usage:

1. Pull up a terminal or SSH into the target server.

2. Logon as root

<code>sudo -i</code>

3. Download the installer script.

<code>wget https://raw.githubusercontent.com/clusterednetworks/ufw-block-http-except-clouldflare/master/cloudflare-ufw.sh</code>

4. Make the script executable

<code>chmod +x cloudflare-ufw.sh</code>

5. Run the script.

<code>./cloudflare-ufw.sh</code>

6. Dont forget to remove your firewall rules that allows "from all http and https".

7. Test your firewall rules.

8. Setup a cronjob to run the script daily/weekly if you choose.
