Educational Keylogger Project
Overview
This repository contains a project aimed at developing educational keyloggers to enhance understanding of keylogging threats, their detection, and mitigation techniques. The project includes implementations of two keylogger tools:

USB Keylogger (Functional): A Python-based implementation designed to log keystrokes when run from a USB device.
PDF Keylogger (Incomplete/WIP): A proof-of-concept for a PDF-based keylogger, which did not produce the desired results.
Disclaimer:
This project is strictly for educational purposes. All testing and usage must occur in controlled environments with proper authorization. Misuse of this project for malicious purposes is prohibited and may violate local laws.

Features
USB Keylogger
Logs keystrokes to a file (Windows10.txt).
Flushes logs to disk periodically or after a character count threshold.
Includes measures to evade simple signature-based detection.
Implements inactivity detection to flush logs after idle periods.
PDF Keylogger (WIP)
Generates a PDF containing embedded JavaScript.
Intended to demonstrate potential exploitation via PDF files.
Note: This tool did not achieve its intended functionality and is for illustrative purposes only.
Project Files
Keylogger Implementations
USB Keylogger:
Code available in usbkey.txt. Outputs logs to Windows10.txt.
PDF Keylogger:
Code available in pdfkey.txt. Results are not functional as intended.
Auxiliary Files
Server: server.txt contains a Flask application to simulate a server for receiving keylogging data.
Keylogger Core: keylogger.txt contains a simplified keylogging script.
Requirements
Dependencies
The project is built with Python and requires the following libraries:

pynput
reportlab
PyPDF2
flask
requests
Installation
Clone this repository:
bash
Copy code
git clone https://github.com/<your-username>/educational-keyloggers.git
cd educational-keyloggers
Install dependencies:
bash
Copy code
pip install -r requirements.txt
Usage
USB Keylogger
Run the script:
bash
Copy code
python usbkey.txt
Keystrokes will be logged to Windows10.txt.
PDF Keylogger
Modify the ngrok URL in pdfkey.txt to your server endpoint.
Generate the PDF:
bash
Copy code
python pdfkey.txt
Open the generated PDF to observe its behavior. (Results are currently incomplete.)
Ethical Considerations
Ensure proper authorization before testing.
Conduct all testing in isolated, controlled environments.
Educate users about potential threats and mitigation techniques.
Known Issues
PDF Keylogger: The tool did not achieve the desired functionality. It remains a proof of concept for educational purposes.
Server Simulation: The Flask server (server.txt) is basic and intended for demo purposes only.
Contribution
Contributions are welcome! Please follow the CONTRIBUTING.md for guidelines.

License
This project is licensed under the MIT License. See LICENSE for details.

Disclaimer
This repository is for academic purposes only. The author is not responsible for any misuse of the provided code.


