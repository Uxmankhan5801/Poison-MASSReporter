![image](https://github.com/ParzivalHack/Poison-MASSReporter/assets/82817793/1ba11691-d476-4d25-bbca-0f0ef40f8027)


# Poison MASSReporter

This script is a PyQt5-based application that performs a Mass Reporting Attack on any TikTok profile, resulting in a ban for most of them.
The tool is intended to automate the reporting of TikTok profiles by sending HTTP requests to a Inspect Element/Network URL, using random User-Agent strings and Accept-Language headers. The reporting process runs on a separate thread and provides real-time updates on the number of reports sent, user-agent, and accept-language used. The GUI allows users to input the target URL and easily initiate the reporting process.

# Features

* Multithreaded Reporting:
The script utilizes multithreading to execute the reporting process in a separate thread. This design ensures that the GUI remains responsive during the reporting operation, preventing it from freezing due to resource-intensive tasks.

* User-Agent Randomization:
The application selects a user-agent from an assortment of pre-defined user-agent strings for each HTTP request. This randomization imitates various device and browser types, making the requests appear diverse and less predictable.

* Accept-Language Variation:
To mimic real-world scenarios, the tool employs a random selection of accept-language headers from a predefined list. This feature enables the application to present itself as originating from different languages and locales.

* Dynamic Reporting Statistics:
During the reporting process, the application computes and displays real-time statistics, including the total number of reports sent, the rate of reporting in reports per minute (reports/min) and the headers used for each specific request. These metrics offer insight into the progress and intensity of the reporting operation.

* Responsive Graphical User Interface (GUI):
The GUI is constructed using the PyQt5 library, ensuring a visually pleasing and user-friendly interface. Users can input the target URL and initiate the reporting process with a single button click. This design promotes readability, maintainability, and scalability.

* Output Visualization:
The application maintains an output text box within the GUI to present the reporting progress and outcomes. This enables users to view the ongoing reporting status, including success and failure reports.

* Target URL Input:
Users can input the target URL where the reporting requests are directed. The application validates the URL and ensures that a valid URL is provided before initiating the reporting process.

* Graceful Handling of Invalid Input
The script incorporates robust input validation, notifying users when an invalid or empty target URL is provided. This prevents accidental or erroneous execution of the reporting process.

* Error Handling:
The script employs effective error handling mechanisms to address potential issues such as failed HTTP requests. Error messages are communicated to the user interface to ensure transparency in the reporting process.

# Proof of Concept (POC)
![image](https://github.com/ParzivalHack/Poison-MASSReporter/assets/82817793/ca89eef8-281b-4b56-9a04-f30c312132a1)
DISCLAIMER:
The tool's effectiveness, solely depends on TikTok's algorithm. No results are guaranteed. Use this tool responsibly and following TikTok's guidelines/ToS.

# Download Prerequisites

* ```pip install requests```
* ```pip install pyqt5```

# Linux & MacOS

* ```git clone https://github.com/ParzivalHack/Poison-MASSReporter```
* ```cd Poison-MASSReporter```
* ```python poison.py```

# Windows
* Search in your pc the "Microsoft Store" and, once opened, search "Python" and install "Python 3.10".
* Just download the files in this repository (only poison.py and the run.bat file) and be sure to keep them all in the same directory on your pc (i suggest putting them directly on your Desktop).
* Double-click on the run.bat file to execute the tool.
* Open TikTok on your browser, login with your account and go on the target's profile
* Open Inspect Element, go on the ">>" and then click on "Network" (see image below for reference)
![image](https://github.com/ParzivalHack/Poison-MASSReporter/assets/82817793/9134205f-6d08-46ce-8f5a-f6368c6e69a3)
* Once there, just normally report (1 time is enough) the Target and check the Inspect Element/Network for an URL like the one below (in the Inspect Element, the URL, just starts with "?aid="):
https://www.tiktok.com/aweme/v2/aweme/feedback/?aid=1988&app_language=it-IT&app_name=tiktok_web&browser_language=it-IT&browser_name=Mozilla&browser_online=true&browser_platform=Win32&browser_version=5.0%20%28Windows%20NT%2010.0%3B%20Win64%3B%20x64%29%20AppleWebKit%2F537.36%20%28KHTML%2C%20like%20Gecko%29%20Chrome%2F114.0.0.0%20Safari%2F537.36%20OPR%2F100.0.0.0&channel=tiktok_web&cookie_enabled=true&current_region=IT&device_id=7264255513738053152&device_platform=web_pc&focus_state=true&from_page=user&history_len=7&is_fullscreen=false&is_page_visible=true&lang=it-IT&nickname=sticazzi&object_id=134791939023036416&os=windows&owner_id=134791939023036416&priority_region=IT&reason=9007&referer=https%3A%2F%2Fwww.tiktok.com%2Flogin%2Femail%2Fforget-password&region=IT&report_type=user&reporter_id=7093583201461322757&root_referer=https%3A%2F%2Fwww.tiktok.com%2Flogin%2Femail%2Fforget-password&screen_height=960&screen_width=1536&secUid=MS4wLjABAAAAN4yo9KTjQofc42djUQyOIqsFXm6lKoDeBkY4llMgc2CPILEt4FT-SrG9vZG94Su-&target=134791939023036416&tz_name=Europe%2FRome&verifyFp=verify_lkzpdqth_JSVAd8B4_OvvF_4oDS_BMmY_qZoyjfADU0eT&webcast_language=it-IT
* Now, just input the URL in the tool and start MASS Reporting :D

# License AGPL-3.0

Features of the GNU Affero General Public License (AGPL-3.0):

* Copyleft: Like the GPL, the AGPL-3.0 is a copyleft license. This means that if you modify or extend the software licensed under AGPL-3.0, you must distribute those modifications under the same license. This ensures that the source code remains open and accessible to everyone.

* Network Interaction: One key feature that distinguishes the AGPL-3.0 from the regular GPL is its "network interaction" clause. If you run a modified AGPL-licensed software on a server and provide access to it over a network, you must also make the modified source code available to the users who interact with that software over the network. This closes the so-called "application service provider (ASP) loophole" that exists in the regular GPL.

* Distribution and Use: AGPL-3.0 allows users to freely use, modify, and distribute the software, provided they comply with the license's terms, including the distribution of the source code for any changes.

* Compatibility: The AGPL-3.0 is not compatible with all other open-source licenses, particularly those that do not require derivative works to be distributed under the same license. If you use AGPL-3.0 code in your project, your project must be released under AGPL-3.0 or a compatible license.
