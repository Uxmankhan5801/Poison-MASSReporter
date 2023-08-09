![image](https://github.com/ParzivalHack/Poison-MASSReporter/assets/82817793/956fb0cb-6000-46d3-8426-a01e07c15a42)

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
