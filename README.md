# LFI Suite

<h3> What is LFI Suite? </h3>

LFISuite is an open source local file inclusion scanner and exploiter that is coded in Python. It supports multiple attack points and also has TOR proxy support. We all know that Local File Inclusion (also known as LFI) is a process of “including” locally present files, through the exploitation of vulnerable inclusion procedures implemented in the application that accepts un-sanitized input.LFI Suite is a totally automatic tool able to scan and exploit Local File Inclusion vulnerabilities using many different methods of attack.

# Output
![alt tag](https://telegra.ph/file/65786a01fdb870f6e52b8.png)

* * * 

<h3> Features </h3>

* Works with Windows, Linux and OS X
* Automatic Configuration 
* Automatic Update
* Provides 8 different Local File Inclusion attack modalities:
  - /proc/self/environ
  - php://filter
  - php://input
  - /proc/self/fd
  - access log
  - phpinfo
  - data://
  - expect://

* Provides a ninth modality, called <b>Auto-Hack</b>, which scans and exploits the target automatically by trying all the attacks one after the other without you having to do anything (except for providing, at the beginning, a list of paths to scan, which if you don't have you can find in this project directory in two versions, small and huge). 
* Tor proxy support
* Reverse Shell for Windows, Linux and OS X


<h3> How to use it? </h3>

Usage is extremely simple and LFI Suite has an easy-to-use user interface; just run it and let it lead you.
##### Reverse Shell
When you got a LFI shell by using one of the available attacks, you can easily obtain a reverse shell by entering the command <b>"reverseshell"</b> (obviously you must put your system listening for the reverse connection, for instance using <b>"nc -lvp port"</b>).

<h3> Dependencies </h3>

* Python <b>2.7</b>.x
* Python extra modules: termcolor, requests
* socks.py 

> When you run the script, in case you are missing some modules, it will check if you have <b>pip</b> installed and, in case you don't, it will install it <b>automatically</b>, then using pip it will install also the missing modules and download the necessary file <b>socks.py</b>.<br>I tried it on different operating systems (Debian,Ubuntu,Fedora,Windows 10,OS X) and it worked great, but if something strange happens to you and the automatic installation of pip and other modules fails, please install missing modules manually and re-run the script.
<br>![#f03c15](https://placehold.it/15/f03c15/000000?text=+) <b>IMPORTANT: In order to allow the script to install missing modules (and in case pip) automatically, you MUST run the script as root (or, at least, with sufficient permissions) the first time.</b>


<h3> Disclaimer </h3>

I am not responsible for any kind of illegal acts you cause. This is meant to be used for project. If you plan to copy, redistribute please give credits to the original author i.e., <<b>d35m0nd142@gmail.com</b>>.

