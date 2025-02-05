# DDos-Attack
![img_1.png](img_1.png)
## What Is A DDos-Attack
A Distributed Denial of Service (DDoS) attack is an attempt to make an online service unavailable by overwhelming it with traffic from multiple sources. These attacks target a wide variety of important resources, including banks, news websites, and other critical infrastructure. DDoS attacks present a major challenge to ensuring the availability and reliability of online services.

## Types of DDoS Attacks
There are several types of DDoS attacks, including:
- **Volume-Based Attacks**: These attacks aim to consume the target's bandwidth by sending a massive amount of traffic. Examples include UDP Flood, ICMP Flood, and HTTP Flood.
- **Protocol Attacks**: These attacks exploit vulnerabilities in network protocols to exhaust the target's resources. Examples include SYN Flood and Ping of Death.
- **Application Layer Attacks**: These attacks target specific applications or services running on the target server. Examples include HTTP GET/POST floods and Slowloris attacks.

## Description of This Script
This script implements a **UDP Flood** attack, which is a type of volume-based DDoS attack. It sends a large number of UDP packets to the target IP address and port, attempting to overwhelm the target system's resources.

### How It Works
1. **Initialization**:
   - Creates a UDP socket.
   - Generates a random payload of 1490 bytes.
   - Prompts the user to input the target IP address and port.

2. **Attack Execution**:
   - Enters an infinite loop where it continuously sends UDP packets to the target.
   - Increments the port number after each packet, cycling through all valid ports (1–65534).

3. **Output**:
   - Prints the number of packets sent, the target IP, and the current port.

### Limitations
- **Bandwidth Constraints**: The attacker's internet connection speed limits the volume of traffic they can send.
- **Firewall and IDS/IPS**: Modern networks often have firewalls and IDS/IPS that can detect and block such attacks.
- **Port Increment Logic**: The script increments the port number after each packet, reducing its focus on a single port, potentially making it less effective.

## Download And Install
**Note**: This script is for educational purposes only and should not be used for malicious intent.

```sh
git clone https://github.com/Prarambha369/DDos-Attack.git
```
```sh
cd DDos-Attack
```
```sh
chmod +x ddos-attack.py
```
```sh   
python ddos-attack.py
```
## Usage

1. Run the script:
    ```sh
    python ddos-attack.py
    ```
2. Enter the target IP address and port when prompted.
3. The script will start sending a flood of requests to the target IP address.
4. To stop the attack, press `Ctrl + C`.

## Disclaimer
This tool is for educational purposes only. Use it responsibly and do not use it to attack any website without permission. Unauthorized use of this tool is illegal and unethical. The target website will be down for a while. Use this tool responsibly and do not use it to attack any website without permission. Unauthorized use of this tool is illegal and unethical. The author is not responsible for any misuse of this tool. Use it at your own risk. Enjoy!

## Author

MrBashyal

GitHub: [Prarambha369](https://github.com/Prarambha369)

## ScreenShot

![Screenshot](img.png)