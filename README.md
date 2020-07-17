# ufw-block-http-except-clouldflare
This is a shell script that will get cloudflares IP Block and then generate a ufw allow command
This script is designed for debian based linux servers using the UFW (Uncomplicated Firewall)

# Usage:

1. Pull up a terminal or SSH into the target server.
2. Logon as root
<code>sudo -i</code>
3. Download the installer script.
<code>wget https://raw.githubusercontent.com/clusterednetworks.com/ufw-block-http-except-clouldflare
/master/cloudflare-ufw.sh</code>
4. Make the script executable
<code>chmod +x cloudflare-ufw.sh</code>
5. Run the script.
<code>./cloudflare-ufw.sh</code>
6. Dont forget to remove your firewall rules that allows "from all http and https"
7. Test
