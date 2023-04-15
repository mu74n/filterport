#filterport

Is a complementary tools for Nmap scanner. When we do a scan with nmap (for example, solving a machine in HackTheBox) we can save time if the port numbers are arranged in such a way that they are easy to copy.
This is useful when we start with SYN Scan and then want to launch a list of reconnaissance scripts to get more information about the services running on the ports. Or any other type of use

Before running it, you should do a scan with nmap. The suggested command is:
nmap -sS -p- --open <iptarget> -oG <filename>

Add more parameters if necessary

If you have permission denied to execute the file. You just have to locate yourself in the path where you have the downloaded file and execute a chmod +x filterport.
If you copy the file to any of the paths you can see by running the command:
echo $PATH
Then you won't have to look for the file path to run the command

Usage example (In local directory):
./filterport <filename>

If the file is included in any of the $PATH directories, we remove the "./":
filterport <filename>
