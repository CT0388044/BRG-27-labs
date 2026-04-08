| **Student Name:**           | Khaidhir Danish                            |
|-----------------------------|--------------------------------------------|
| **Student ID:**             | CT0388044                                  |
| **GitHub Repository Link:** | <https://github.com/CT0388044/BRG-27-labs> |

**Upload DocX File – Reflective Journal report to Kaplan LMS:**

**FileName: CT0388044_Khaidhir_Danish_Reflective_Journal.docx**

**upload to SharePoint site:
[Video]([https://m365kloud.sharepoint.com/:f:/s/LEARN/IgC9M06IRir2RJyC8lWbgg24AVfTSltgiCIbQdYKIcroiVU?e=Uh4ebF](https://m365kloud.sharepoint.com/sites/LEARN/_layouts/15/stream.aspx?id=%2Fsites%2FLEARN%2FShared%20Documents%2Fe%2DKAPLAN%2FMU%2DISEABRG%2D27%2DIntroServer%2Fstudent%2FVideoUpload%2FCt0388044%20Khaidhir%20Danish%20AssignmentISEA%2Emp4&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E5c7c5570%2D2848%2D441b%2Da232%2D1816725ca898))**

**Video Walkthrough Filename: FileName:
Ct0388044_Khaidhir_Danish_AssignmentISEA.mp4**

# Contents

[1. Introduction]

[2. Linux Environment Setup and GitHub Integration]

[Lab 1a-1]

[3. Linux Services, Permissions, and Bash Scripting]

[Lab 1a-2]

[Lab1b-1]

[Lab1b-2]

[Lab 1b-3]

[4. Cloud Infrastructure and TCO Analysis]

[Lab2a-1]

[Lab2b-1]

[Lab2b-2]

[5. DNS Setup and SSL Configuration]

[Lab3a-1]

[Lab3a-2]

[6. Automation and Cron Jobs]

[Lab3b-1]

[7. Additional Server Service]

[8. Problems Encountered and Solutions]

[9. Industry Relevance]

[10. Final Reflection]

[11. AI Tools Used (if any)]

(each heading will be bookmarked and link to the content page and vice
versa)

### [1. Introduction]

This reflection journal will be on my journey doing the lab work and a
few challenges set by that lab activities. I will be setting up a
VirtualBox for a desktop environment for Ubuntu Linux. Then I will get
introduced to Linux terminal commands. Next, I will setting up Linux
services, permissions, searching filesystems, and add additional users.
I will learn Bash Coding for automated scripting. Finally, I will use
AWS EC2 service to host a cloud VM to host a public website while
learning more on DNS and obtaining a digital certificates for the
website.

### [2. Linux Environment Setup and GitHub Integration]

#### GitHub Usage

### [<span id="_Toc226552343" class="anchor"></span>Lab 1a-1]

To setup VirtualBox, I need to install from their website,
<https://www.virtualbox.org/wiki/Downloads>

<img src="media/image1.png" style="width:4.14786in;height:1.9144in" />

<img src="media/image2.png" style="width:4.11964in;height:3.16763in" />

Then, I need to download Lubuntu desktop image,
<https://cdimage.ubuntu.com/lubuntu/releases/noble/release/>

<img src="media/image3.png" style="width:4.14923in;height:2.16372in" />

This is to set up virtualbox and mount Ubuntu ISO

<img src="media/image4.png" style="width:6.11434in;height:5.17628in" />

I set up 8192 MB RAM, 2 CPUs cores, 25 GB Disk Size for the VirtualBox
and called it ISEA

<img src="media/image5.png" style="width:5.90591in;height:5.78287in" />

After booting up, I need to install Lubuntu.

<img src="media/image6.png" style="width:4.1431in;height:2.58147in" />

It gave me an error for not plugging in my host pc which is a laptop

<img src="media/image7.png" style="width:4.12464in;height:2.56865in" />

Once host PC is connected to power, I reset VirtualBox and boot up. Then
I continue with the installation

<img src="media/image8.png" style="width:4.15081in;height:2.56898in" />

<img src="media/image9.png" style="width:4.14204in;height:2.58568in" />

<img src="media/image10.png" style="width:4.14376in;height:1.48618in" />

<img src="media/image11.png" style="width:4.1448in;height:3.01517in" />

I created a user called khaidhir.

<img src="media/image12.png" style="width:4.16952in;height:2.58413in" />

### [3. Linux Services, Permissions, and Bash Scripting](#content)

### Lab 1a-2

ps -e OR ps -A means list running process on the system, across all
users and terminals

<img src="media/image13.png" style="width:4.12769in;height:3.60555in" />

top means interactive viewer for process viewing

<img src="media/image14.png" style="width:4.1991in;height:2.52215in" />

1 to list all CPUs cores

<img src="media/image15.png" style="width:4.1538in;height:0.76375in" />

q to quit

htop for alternative interactive viewer for process viewing

<img src="media/image16.png" style="width:6.18267in;height:3.27695in" />

ls means list directory contents

<img src="media/image17.png" style="width:4.23822in;height:0.36269in" />

ls -la is list all with details by showing hidden files

<img src="media/image18.png" style="width:4.14197in;height:2.5874in" />

-h is to change the files sizes in KB, MB or GB format for human
readability

ls -lah

<img src="media/image19.png" style="width:4.12544in;height:3.18355in" />

ls -alt is to order the list by most recently modified first

<img src="media/image20.png" style="width:6.5in;height:4.44167in" />

clear to clear the terminal

touch is to create an empty file

touch \<filename\>

touch testfile is to create an empty testfile

<img src="media/image21.png" style="width:4.12333in;height:0.41101in" />

they will appear at khaidhir folder

<img src="media/image22.png" style="width:4.14294in;height:2.88678in" />

gedit is a graphical text editor

gedit \<filename\>

gedit testfile

My system has not installed gedit yet.

sudo means to run the command as root

apt to install debian packages

install gedit means to install a program called gedit

The command sudo apt install gedit is to install gedit

<img src="media/image23.png" style="width:4.23493in;height:0.66058in" />

Whenever using sudo, I need to enter user password

<img src="media/image24.png" style="width:4.246in;height:0.61558in" />

A confirmation screen from apt to install gedit and its dependecies.

<img src="media/image25.png" style="width:4.16844in;height:3.80904in" />

gedit testfile will open testfile with the editor

<img src="media/image26.png" style="width:4.13444in;height:3.54077in" />

I will type a section from an online article from Google into testfile
and save file.

<img src="media/image27.png" style="width:4.15041in;height:0.9569in" />

nano is a terminal-based text editor

nano \<filename\>

nano testfile to open a text editor

<img src="media/image28.png" style="width:4.15098in;height:2.35976in" />

Ctrl + x to exit the text editor

cat is to display content in the terminal

cat \<filename\>

cat testfile

<img src="media/image29.png" style="width:6.10708in;height:0.76991in" />

less is to display content in pagination

less \<filename\>

less testfile

<img src="media/image30.png" style="width:5.99975in;height:0.8051in" />

type q to exit

cp is to copy file current source file into a destination file. If
destination file does not exist, it will be created

cp \<(source)filename\> \<(destination)filename\>

cp testfile testfile2 means to copy testfile contents into testfile2

and ls to list khaidhir directory contents

<img src="media/image31.png" style="width:4.18259in;height:0.72793in" />

<img src="media/image32.png" style="width:4.14119in;height:3.04351in" />

cat testfile2 to see the copied contents

<img src="media/image33.png" style="width:6.5in;height:2.09653in" />

mv is to move or rename

mv \<(old)filename\> \<(new)filename\> is to rename

mv \<filename\> \</destination\> is to move

mv testfile2 testfile3

<img src="media/image34.png" style="width:4.1902in;height:0.73866in" />

<img src="media/image35.png" style="width:4.1459in;height:3.14884in" />

uname is to show kernel info

uname -a

<img src="media/image36.png" style="width:6.01942in;height:0.43731in" />

lsb_release is to show operating system info

lsb_release -a

<img src="media/image37.png" style="width:4.19712in;height:1.31698in" />

hostnamectl is to show hostname and system info

<img src="media/image38.png" style="width:4.15218in;height:2.77211in" />

whoami is to see current user

<img src="media/image39.png" style="width:4.17418in;height:0.45805in" />

adduser danish will have an error that a root user may add a new user

<img src="media/image40.png" style="width:4.28606in;height:0.5092in" />

sudo whoami to see as current root user

<img src="media/image41.png" style="width:4.18359in;height:0.83672in" />

sudo adduser \<username\> is to add a new user into the system as a root
user

sudo adduser danish

Then danish user need to set a password and key in details

<img src="media/image42.png" style="width:5.92337in;height:3.51921in" />

ip a is to show IP addresses

<img src="media/image43.png" style="width:6.08267in;height:2.2615in" />

ping 8.8.8.8

<img src="media/image44.png" style="width:4.13268in;height:3.00591in" />

Ctrl + c to exit the ping

cat /etc/hosts

<img src="media/image45.png" style="width:4.11656in;height:1.6088in" />

ping localhost

<img src="media/image46.png" style="width:4.13453in;height:2.63134in" />

to edit hosts file in gedit

<img src="media/image47.png" style="width:4.23116in;height:0.33904in" />

add 8.8.8.8 GoogleEpicDNS

<img src="media/image48.png" style="width:4.14773in;height:1.7198in" />

ping GoogleEpicDNS

<img src="media/image49.png" style="width:4.14678in;height:2.32016in" />

nslookup google.com is used to query DNS and find out which IP addresses
a domain name resolves to. There are multiple ip addresses because
google uses multiple servers or DNS does geo-routing & load balancing to
improve speed and reliability

<img src="media/image50.png" style="width:4.14785in;height:4.45584in" />

sudo apt install whois is to look up ownership and registration
information for domain names

whois murdoch.edu.sg

<img src="media/image51.png" style="width:5.92565in;height:3.53576in" />

lsusb to list USB devices connected to the system

<img src="media/image52.png" style="width:4.15159in;height:0.70391in" />

lspci to list PCI devices connected to the system

<img src="media/image53.png" style="width:5.93522in;height:1.49776in" />

cat /proc/cpuinfo

<img src="media/image54.png" style="width:5.91404in;height:3.18196in" />

GUI version at VirtualBox

<img src="media/image55.png" style="width:4.16602in;height:2.76889in" />

lsusb \> output_of_lsusb is to save the output into a file called
output_of_lsusb

<img src="media/image56.png" style="width:4.1755in;height:0.90335in" />

less output_of_lsusb

<img src="media/image57.png" style="width:4.187in;height:0.62581in" />

cat output_of_lsusb

<img src="media/image58.png" style="width:4.18534in;height:0.71589in" />

ls -la output_of_lsusb

<img src="media/image59.png" style="width:4.23281in;height:0.44001in" />

181 byte

rm is to delete file

rm \<filename\>

rm output_of_lsusb

<img src="media/image60.png" style="width:4.13835in;height:0.7839in" />

<img src="media/image61.png" style="width:4.17649in;height:0.67645in" />

Now to download Brave browser, the website gives a command code to run
for installation.

To paste in terminal is Ctrl + Shift + v

<img src="media/image62.png" style="width:4.18154in;height:2.02956in" />

sudo apt install curl

<img src="media/image63.png" style="width:4.16894in;height:1.12864in" />

sudo curl -fsSLo /usr/share/keyrings/brave-browser-archive-keyring.gpg
https://brave-browser-apt-release.s3.brave.com/brave-browser-archive-keyring.gpg

sudo curl -fsSLo /etc/apt/sources.list.d/brave-browser-release.sources
https://brave-browser-apt-release.s3.brave.com/brave-browser.sources

<img src="media/image64.png" style="width:4.19385in;height:0.73751in" />

sudo apt update

<img src="media/image65.png" style="width:4.16442in;height:2.07242in" />

sudo apt install brave-browser

Brave browser has been successfully installed in VirtualBox

<img src="media/image66.png" style="width:1.71899in;height:1.44812in" />

<img src="media/image67.png" style="width:4.12473in;height:3.18168in" />

My Ubuntu Plasma Discover doesn’t work. I tried opening Discover from
terminal,

plasma-discover

I tried,

sudo apt update

sudo apt upgrade

Then,

sudo apt remove plasma-discover

sudo apt install plasma-discover

sudo reboot

Next, I try to install Gnome software

sudo apt update

sudo apt install gnome-software

Then, open it by terminal.

gnome-software. Then, I install Oneko. A desktop widget that follows the
cursor around

<img src="media/image68.png" style="width:4.13329in;height:1.43473in" />

<img src="media/image69.png" style="width:4.14153in;height:2.76854in" />

sudo apt install build-essential

I created hello_world.c and edit using gedit

<img src="media/image70.png" style="width:5.86943in;height:3.57684in" />

There is a syntax error witth my code, I wrote “prinf” instead of
“printf”

gcc hellow_world.c -o hello_world_executable to compile hello_world.c

./hello_world_executable to run the c program

<img src="media/image71.png" style="width:4.15268in;height:0.65485in" />

cat hello_world.c vs cat hello_world_executable

<img src="media/image72.png" style="width:4.17012in;height:1.26797in" />

<img src="media/image73.png" style="width:5.87648in;height:4.91779in" />

### [<span id="_Toc226552346" class="anchor"></span>Lab1b-1](#content)

sudo apt update

<img src="media/image74.png" style="width:4.17022in;height:1.47651in" />

sudo apt install nginx-full

<img src="media/image75.png" style="width:5.95495in;height:3.22115in" />

sudo apt install nmap

<img src="media/image76.png" style="width:4.5582in;height:2.36481in" />

sudo apt install openshh-server

<img src="media/image77.png" style="width:5.90184in;height:3.08207in" />

Typing <http://127.0.0.1/> into firefox browser

<img src="media/image78.png" style="width:4.14173in;height:3.30851in" />

ip a

<img src="media/image79.png" style="width:4.16668in;height:2.45549in" />

gedit /var/www/html/index.nginx-debian.html

<img src="media/image80.png" style="width:5.91964in;height:3.56823in" />

No permission error if so type sudo at the start of the line

nano is to use the terminal to edit the file

while gedit is to use the graphical text editor

to view VirtualBox Nginx from host computer

sudo systemctl status nginx to check if nginx is running

<img src="media/image81.png" style="width:5.9271in;height:3.52586in" />

ip a to find VirtualBox ip address. My virtualBox ip address is
10.0.2.15

<img src="media/image82.png" style="width:6.06194in;height:0.81344in" />

set up NAT port forwarding

Go to VirtualBox network settings and set up port forwarding

Add a rule:

Name: nginx

Protocol: TCP

Host Port: 8080

Guest Port: 80

<img src="media/image83.png" style="width:5.97032in;height:3.94258in" />

open localhost:8080 in host computer

<img src="media/image84.png" style="width:5.87718in;height:3.46917in" />

to ping from VirtualBox to host pc.

shutdown VirtualBox

add another network adapter

Attached to: Host-onlt Adapter

Name: VirtualBox Host-Only Ethernet Adapter

<img src="media/image85.png" style="width:4.18239in;height:2.77039in" />

ip a to check VirtualBox ip address which is 192.168.56.101

<img src="media/image86.png" style="width:4.29293in;height:1.03792in" />

ping from host PC to VirtualBox

<img src="media/image87.png" style="width:4.13035in;height:2.33524in" />

ping from host VirtualBox to PC

<img src="media/image88.png" style="width:4.15246in;height:3.05667in" />

nmap 192.168.56.101

nmap 10.0.2.15

<img src="media/image89.png" style="width:4.10568in;height:2.50683in" />

nmap 127.0.0.1

<img src="media/image90.png" style="width:4.14426in;height:1.16004in" />

sudo apt remove nginx-full

sudo apt autoremove

nmap 127.0.0.1

<img src="media/image91.png" style="width:4.22154in;height:1.42973in" />

sudo apt install nginx-full

<img src="media/image92.png" style="width:4.10749in;height:1.36741in" />

sudo ufw status verbose

<img src="media/image93.png" style="width:4.15465in;height:0.28097in" />

sudo ufw enable

sudo ufw status verbose

<img src="media/image94.png" style="width:4.14626in;height:1.12649in" />

sudo ufw allow 80/tcp

From host PC

<img src="media/image95.png" style="width:4.19335in;height:1.59849in" />

sudo ufw deny 80/tcp

from host PC

<img src="media/image96.png" style="width:4.12005in;height:1.41473in" />

from host PC, can’t access localhost:8080

<img src="media/image97.png" style="width:4.13334in;height:2.19738in" />

cat /etc/passwd

I have created danish user

<img src="media/image98.png" style="width:6.5in;height:0.46597in" />

ssh <danish@192.168.56.101>

<img src="media/image99.png" style="width:5.52816in;height:4.16502in" />

dir -la on danish user

<img src="media/image100.png" style="width:5.42129in;height:3.7532in" />

exit to log out

wget https://gutenberg.org/files/76/76-0.txt

<img src="media/image101.png"
style="width:5.81065in;height:1.30305in" />

wget https://gutenberg.org/files/36/36-0.txt

<img src="media/image102.png" style="width:6.5in;height:1.44861in" />

wget https://gutenberg.org/files/12/12-0.txt

<img src="media/image103.png" style="width:6.5in;height:1.47361in" />

mkdir books

<img src="media/image104.png"
style="width:4.14604in;height:3.73498in" />

mv 76-0.txt 36-0.txt 12-0.txt books

<img src="media/image105.png"
style="width:3.49605in;height:3.75303in" />

tar cf books.tar books

<img src="media/image106.png" style="width:4.22168in;height:2.8361in" />

bzip2 books.tar

<img src="media/image107.png"
style="width:4.18147in;height:2.80641in" />

ls -lh

<img src="media/image108.png"
style="width:4.26889in;height:0.60294in" />

however books storage is not 4.0KB. 4.0KB is just the size of the
metadata<img src="media/image109.png"
style="width:4.17218in;height:4.85667in" />

therefore use, du -sh books to see the real size

<img src="media/image110.png"
style="width:4.16018in;height:0.42687in" />

Challenge 1

ssh danish@192.168.54.101

<img src="media/image111.png"
style="width:4.12534in;height:1.23628in" />

touch Hi_danish

ls -l

<img src="media/image112.png" style="width:4.13287in;height:2.1914in" />

Challenge 2

gedit Hi_danish

<img src="media/image113.png" style="width:4.21572in;height:0.5675in" />

Challenge 3

<img src="media/image114.png"
style="width:4.21442in;height:2.83888in" />

Challenge 4

<img src="media/image115.png"
style="width:4.13281in;height:0.68394in" />

<img src="media/image116.png"
style="width:4.12042in;height:2.27635in" />

### [<span id="_Toc226552347" class="anchor"></span>Lab1b-2](#content)

ad d Alice, Bob, and Mallory users

sudo adduser alice

sudo adduser bob

sudo adduser mallory

<img src="media/image117.png"
style="width:4.14005in;height:0.57235in" />

Create group for sharing

Add users to the group

sudo adduser alice forSharing

sudo adduser bob forSharing

<img src="media/image118.png"
style="width:3.78178in;height:0.32296in" />

Create folders and files for sharing

sudo mkdir /home/shared

sudo touch /home/shared/file1.bat

sudo touch /home/shared/file2.exe

sudo touch /home/shared/file3.txt

sudo touch /home/shared/file4.md

sudo touch /home/shared/file5.deb

<img src="media/image119.png"
style="width:4.20671in;height:1.00539in" />

<img src="media/image120.png"
style="width:4.18265in;height:3.96548in" />

ls -l /home/shared

<img src="media/image121.png" style="width:4.1935in;height:1.49147in" />

Set Alice the owner and forSharing the group

sudo chown -R alice:forSharing /home/shared

<img src="media/image122.png" style="width:4.21343in;height:0.4362in" />

Set permission

7 rwx

5 r-x

0 ---

sudo chmod -R 750 /home/shared

<img src="media/image123.png" style="width:4.1656in;height:0.26925in" />

ls -ld /home/shared

<img src="media/image124.png" style="width:4.1702in;height:0.44999in" />

testing for alice

Alice can read, write, and execute

<img src="media/image125.png"
style="width:4.00787in;height:1.64126in" />

testing for bob

Bob can read and execute but cannot write

<img src="media/image126.png" style="width:4.1866in;height:1.72563in" />

testing for mallory

Mallory cannot access the directory at all

<img src="media/image127.png" style="width:4.1877in;height:1.45898in" />

To add Mallory to the sudo group

sudo usermod -aG sudo mallory

<img src="media/image128.png"
style="width:4.18934in;height:2.91374in" />

remove directory

<img src="media/image129.png"
style="width:4.15641in;height:0.70162in" />

### [<span id="_Toc226552348" class="anchor"></span>Lab 1b-3](#content)

From host PC, I’ll transfer 1b-3-Gutenberg.zip file to VirtualBox using
scp

<img src="media/image130.png"
style="width:4.22244in;height:0.51066in" />

Now VirtualBox has the file

<img src="media/image131.png" style="width:4.2276in;height:0.68427in" />

To unzip .zip files, I need to check if my VirtualBox have unzip

<img src="media/image132.png"
style="width:4.14331in;height:2.09468in" />

unzip 1b-3-Gutenberg.zip

<img src="media/image133.png"
style="width:4.18775in;height:1.06126in" />

find /home/khaidhir/1b-3-Gutenberg - name “\*.txt”

<img src="media/image134.png"
style="width:4.15861in;height:0.73131in" />

find /home/khaidhir/1b-3-Gutenberg means to start searching in this
directory

-type f means to search regular files only and no directory

-exec grep -H ‘rejoice’ {} \\

means to search the text ‘rejoice’ and show filename in the output

find /home/khaidhir/1b-3-Gutenberg -type f -exec grep -H ‘rejoice’ {} \\

<img src="media/image135.png"
style="width:4.23584in;height:0.56976in" />

grep -r “rejoice” /home/khaidhir/1b-3-Gutenberg

<img src="media/image136.png"
style="width:4.22363in;height:0.60151in" />

grep -r -C 3 rejoice /home/khaidhir/1b-3-Gutenberg

<img src="media/image137.png"
style="width:5.79365in;height:0.90928in" />

To find recently modified file

find \$1 -type f -exec stat –format ‘%Y :%y %n’ “{}” \\ \| sort -nr \|
cut -d: -f2- \| head

<img src="media/image138.png" style="width:4.1302in;height:1.51705in" />

To find oldest date created file in system

find /home/khaidhir - type f -printf ‘%T+ %p\n’ \| sort \| head -n 20

<img src="media/image139.png" style="width:5.0345in;height:2.43227in" />

To find files size exactly 94 bytes

find /home/khaidhir - type f -size 94c -exec ls {} \\

<img src="media/image140.png"
style="width:5.88578in;height:0.66529in" />

To show the frequency of words inside a file

sed -e ‘s/\s/\n/g’ \< 1b-3-Gutenberg/frankenstein.tzt \| sort \| uniq -c
\| sort -nr \| head -200

<img src="media/image141.png"
style="width:5.91378in;height:2.13364in" />

### [4. Cloud Infrastructure and TCO Analysis](#content)

### [<span id="_Toc226552350" class="anchor"></span>Lab2a-1](#content)

I can’t see the biling yet

<img src="media/image142.png" style="width:5.209in;height:1.90273in" />

I have created a budget alert

<img src="media/image143.png" style="width:6.5in;height:0.81667in" />

### [<span id="_Toc226552351" class="anchor"></span>Lab2b-1](#content)

[Dashboard \| EC2 \|
ap-southeast-2](https://ap-southeast-2.console.aws.amazon.com/ec2/home?region=ap-southeast-2#Home:)

<img src="media/image144.png"
style="width:4.15021in;height:2.11058in" />

ssh -i "websever-key.pem"
<ubuntu@ec2-3-27-65-200.ap-southeast-2.compute.amazonaws.com>

<img src="media/image145.png" style="width:6.5in;height:4.56389in" />

sudo apt update

<img src="media/image146.png" style="width:6.5in;height:0.99236in" />

sudo apt install nginx-full

sudo nano /var/www/html/index.html

<img src="media/image147.png"
style="width:4.87568in;height:2.42742in" />

wget <http://www.eecs.berkeley.edu/Pubs/TechRpts/2009/EECS-2009-28.pdf>

sudo cp EECS-2009-28.pdf /var/www/html/

<img src="media/image148.png"
style="width:4.12815in;height:4.46335in" />

created links in index.html

<img src="media/image149.png" style="width:6.5in;height:0.71875in" />

<img src="media/image150.png"
style="width:3.52195in;height:2.08148in" />
<img src="media/image151.png" style="width:6.5in;height:5.93681in" />

### [<span id="_Toc226552352" class="anchor"></span>Lab2b-2](#content)

mkdir LabFiles

cd LabFiles

touch notes.txt

<img src="media/image152.png" style="width:4.38594in;height:0.7488in" />

echo “This is a Bash scripting lab.” \> notes.txt

cat notes.txt

<img src="media/image153.png" style="width:6.5in;height:1.01319in" />

cp notes.txt backup_notes.txt

<img src="media/image154.png" style="width:6.5in;height:0.80625in" />

mv backup_notes.txt old_notes.txt

<img src="media/image155.png" style="width:6.5in;height:0.79444in" />

rm old_notes.txt

<img src="media/image156.png" style="width:6.5in;height:0.94722in" />

mkdir to create new directory

less or nano

cp is to copy a source file content into destination file content. If
there is no destination file, it will be created.

mv \<(old)filename\> \<(new)filename\> is to rename

mv \<filename\> \</destination\> is to move

nano hello_world.sh

chmod 777 hello_world.sh

<img src="media/image157.png" style="width:4.12552in;height:0.8542in" />

Modifying the echo line

<img src="media/image158.png"
style="width:4.13621in;height:0.94346in" />

<img src="media/image159.png"
style="width:4.21422in;height:0.44618in" />

<img src="media/image160.png"
style="width:4.15789in;height:3.19038in" />

<img src="media/image161.png"
style="width:4.69132in;height:0.34333in" />

<img src="media/image162.png"
style="width:4.14908in;height:2.85249in" />

<img src="media/image163.png"
style="width:4.78848in;height:1.78596in" />

<img src="media/image164.png"
style="width:4.15083in;height:3.75571in" />

<img src="media/image165.png"
style="width:5.26349in;height:0.96835in" />

<img src="media/image166.png"
style="width:4.15931in;height:3.58207in" />

<img src="media/image167.png"
style="width:4.18123in;height:0.26669in" />

<img src="media/image168.png"
style="width:4.10819in;height:3.43534in" />

<img src="media/image169.png"
style="width:3.19565in;height:0.42199in" />

<img src="media/image170.png"
style="width:4.25321in;height:1.79852in" />

free is to display memory usage

-h is to change the files sizes in KB, MB or GB format for human
readability

<img src="media/image171.png" style="width:4.41728in;height:1.0939in" />

<img src="media/image172.png"
style="width:5.20042in;height:3.06358in" />

### [5. DNS Setup and SSL Configuration](#content)

### [<span id="_Toc226552354" class="anchor"></span>Lab3a-1](#content)

I am connected to AWS EC2 VM

<img src="media/image173.png"
style="width:4.16534in;height:3.09152in" />

then I register a new subdomain at FreeDNS

https://freedns.afraid.org/subdomain/

<img src="media/image174.png"
style="width:4.16351in;height:3.40554in" />

<img src="media/image175.png"
style="width:3.34118in;height:1.13943in" />

I check the status of nginx inside AWS EC2 VM

<img src="media/image176.png"
style="width:4.24163in;height:1.80722in" />

Create a new directory and \<insert\>

sudo mkdir /var/www/ISEAlabs

sudo chown -R \$USER:\$USER /var/www/ISEAlabs

Create an index.html file

nano /var/www/ISEAlabs/index.html

<img src="media/image177.png" style="width:6.5in;height:0.78403in" />

sudo nano /etc/ngins/sites-available/ISEAlabs

<img src="media/image178.png" style="width:6.5in;height:1.83194in" />

sudo ln -s /etc/nginx/sites-available/ISEAlabs /etc/nginxsites-enabled/

<img src="media/image179.png"
style="width:4.38028in;height:0.51431in" />

<img src="media/image180.png"
style="width:4.37766in;height:0.66366in" />

Host PC

<img src="media/image181.png" style="width:4.1289in;height:2.29864in" />

### [<span id="_Toc226552355" class="anchor"></span>Lab3a-2](#content)

<https://certbot.eff.org/instructions?ws=nginx&os=snap>

snapd is up and running

<img src="media/image182.png"
style="width:4.35005in;height:2.42692in" />

<img src="media/image183.png" style="width:4.4509in;height:0.42702in" />

<img src="media/image184.png" style="width:4.53371in;height:0.1952in" />

<img src="media/image185.png"
style="width:4.20267in;height:3.74289in" />

now the website doesn’t work

### [6. Automation and Cron Jobs](#content)

### [<span id="_Toc226552357" class="anchor"></span>Lab3b-1](#content)

sudo nano hello_world_test.sh

<img src="media/image186.png"
style="width:4.15056in;height:0.57514in" />

chmod 777 hello_world_test.sh

<img src="media/image187.png"
style="width:4.16867in;height:0.51797in" />

Change the current code using variables

<img src="media/image188.png"
style="width:4.20056in;height:0.78357in" />

<img src="media/image189.png"
style="width:4.28973in;height:0.68562in" />

Change the the code to be arithmetic

<img src="media/image190.png" style="width:4.26704in;height:1.147in" />

<img src="media/image191.png"
style="width:4.09732in;height:0.53318in" />

Doing a for loop

<img src="media/image192.png" style="width:4.28691in;height:1.0218in" />

<img src="media/image193.png"
style="width:4.28535in;height:2.41463in" />

creating files and directories

<img src="media/image194.png"
style="width:4.15779in;height:2.23525in" />

nano /testscript

<img src="media/image195.png"
style="width:4.95262in;height:1.87681in" />

chmod +x testscript

./testscript

<img src="media/image196.png"
style="width:5.51119in;height:2.48993in" />

sudo mv /home/khaidhir/testscript

<img src="media/image197.png"
style="width:5.23387in;height:0.13085in" />

sudo chown khaidhir /usr/bin/testscript

<img src="media/image198.png"
style="width:5.00731in;height:0.13749in" />

setting up for testing

<img src="media/image199.png"
style="width:4.44634in;height:1.17667in" />

testing testscript

<img src="media/image200.png"
style="width:4.16673in;height:2.85128in" />

<img src="media/image201.png"
style="width:4.15142in;height:1.75992in" />

<img src="media/image202.png"
style="width:4.23682in;height:0.44586in" />

checking if zip is installed

zip -v

<img src="media/image203.png"
style="width:4.16204in;height:2.73601in" />

nano testscript

<img src="media/image204.png" style="width:4.14438in;height:2.7523in" />

chmod +x /home/khaidhir/testscript

<img src="media/image205.png"
style="width:4.15535in;height:2.27701in" />

<img src="media/image206.png"
style="width:4.16316in;height:0.92247in" />

### [7. Additional Server Service](#content)

WIREGUARD VPN

sudo apt install wireguard -y

<img src="media/image207.png" style="width:6.5in;height:0.22222in" />

sudo nano /etc/wireguard/wg0.conf

<img src="media/image208.png" style="width:3.7678in;height:1.64559in" />

sudo systemctl enable wg-quick@wg0

sudo systemctl start wg-quick@wg0

<img src="media/image209.png"
style="width:4.16237in;height:3.59671in" />

testing for wireguard connection

<img src="media/image210.png"
style="width:4.11974in;height:1.03742in" />

ip a

<img src="media/image211.png"
style="width:4.35025in;height:0.67438in" />

### [8. Problems Encountered and Solutions](#content)

Can’t connect to EC2 VM after getting Digital cert

- tried checking AWS EC2 security groups, networking and firewall. I
  think to resolve, I need to start a new instance

> Time constraints when dealing with 3 core modules while doing a 2 week
> bridging module.

- need to have a better time management plan

### [9. Industry Relevance](#content)

> I could open up to new job opportunities such as a System
> Administrator, Cloud Engineer / Architect or Network Security
> Specialist.

### [10. Final Reflection](#content)

> The lab exercise is very technical and I appreciate it. I have learn a
> lot from familiarising with command line and scripting.

### [11. AI Tools Used (if any)](#content)

> None
