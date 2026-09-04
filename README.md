# Website-IP-Address-Hostname-Lookup
A simple Python script that retrieves the hostname and IP address of a website entered by the user.  This project uses Python's built-in socket library to resolve a hostname to its corresponding IPv4 address.
✨ Features
🌐 Accepts a website hostname from the user
🔍 Resolves the hostname to an IP address
🖥️ Displays the entered hostname
⚠️ Handles invalid hostnames using socket.gaierror
🐍 Uses only Python's standard library
🛠️ Technologies Used
Python 3
Socket
📦 Requirements

No external Python packages are required.

The script uses the built-in socket module:

import socket
🚀 Installation

Clone the repository:

git clone https://github.com/your-username/website-ip-lookup.git
cd website-ip-lookup

Make sure Python 3 is installed:

python --version
▶️ Usage

Run the script:

python "Get the IP Address and Hostname of A Website(2).py"

The program will ask:

Please enter website address(URL):

Enter a hostname, for example:

google.com
Example Output
Please enter website address(URL):google.com
Hostname: google.com
IP: 142.250.xxx.xxx

The script obtains the IP address using:

socket.gethostbyname(hostname)




⚙️ How It Works

The script follows these steps:

Start
  │
  ▼
Ask for Website Hostname
  │
  ▼
Resolve Hostname
  │
  ▼
Get IP Address
  │
  ├── Success ──► Display Hostname & IP
  │
  └── Failure ──► Display Error

The main functionality is contained inside the get_hostname_IP() function.

⚠️ Error Handling

If the hostname cannot be resolved, the script catches socket.gaierror and displays an error message:

Invalid Hostname, error raised is ...

This prevents the program from terminating unexpectedly when an invalid hostname is entered.

📁 Project Structure
website-ip-lookup/
│
├── Get the IP Address and Hostname of A Website(2).py
└── README.md
🔐 Note

This project performs a basic DNS hostname lookup. It does not perform port scanning, vulnerability scanning, or other security testing.

The result can vary depending on DNS configuration, load balancing, CDNs, and the website's infrastructure.
