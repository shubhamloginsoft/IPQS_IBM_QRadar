# **User Guide:** Farsight DNSDB - IBM QRadar

## Table of Contents
- [Introduction](#1-introduction)
- [Download](#2-download)
- [Installation](#3-installation)
- [Configuration](#4-configuration)
- [Automated Threat Hunting](#5-automated-threat-hunting)
- [Manual Threat Hunting](#6-manual-threat-hunting)

---

## 1. Introduction:

**IPQS Fraud and Risk Scoring** offers a variety of different risk analysis APIs designed to detect and mitigate online threats and abusive behaviour from even the most sophisticated bad actors. Whether its websites of all sizes or enterprise companies, IPQS has the right solutions to solve your challenges. These solutions include online fraud prevention, risk scoring, and threat mitigation. Customizable settings and international data coverage ensures our scoring models perfectly fit your audience.

**IP Reputation & Proxy Detection** service performs real-time lookups to instantly determine how risky a user, click, or transaction is based on an IP address and optional device information. In addition to analysing if the IP address is a proxy or VPN, the API returns over 20 relevant data points such as: 
* Geo location data, 
* ISP,
* Connection type, 
* Device details, 
* Recent reputation activity, 
* Overall fraud score, 
* Status as a proxy,
* VPN, 
* or TOR connection, 
* Abuse Velocity, 
* Other similar data points to classify reputation and risk

**Email Validation & Reputation API** provides real-time email address reputation scoring and validation with hundreds of syntax & DNS checks. The API can be leveraged to determine if the email address exists with the mail service provider and is able to accept new messages. In addition, users are also able to determine if the email address has a poor reputation and associated with any current threats. Lastly, users are able to detect disposable or temporary mail services as well as emails with a history of fraudulent behaviour online.

**Malicious URL Scanner API** scans links and domains in real-time to detect suspicious URLs using trusted machine learning models. These machine learning models can accurately identify phishing links, malware URLs, viruses, parked domains, and suspicious URLs with real-time risk scores. In addition, the machine learning models can confidently classify poor reputation domains, suspicious links, and phishing URLs with a real-time API integration. 

**Phone Number Validation API** Accurately verify phone numbers worldwide and retrieve a combination of carrier and line type details with risk analysis data to assess phone number reputation. IPQS collects phone validation and verification data from a wide variety of carriers and tier 1 telecommunication providers, with support for all regions. Detect inactive and disconnected phone numbers for easy user validation similar to HLR & LRN lookups. Accurately identify virtual and disposable phone numbers along with numbers associated with abusive behavior online.

This document is intended to help users how to download, install and configure the **IPQS Fraud and Risk Scoring** for IBM QRadar. 

**IPQS Fraud and Risk Scoring** for IBM QRadar enables to accelerate incident response with its orchestration and automation capabilities to investigate and mitigate threats. The IBM QRadar users can view the DNS enriched data in the Offense summary page for the Offense Sources. This will help to speed up QRadar investigations and prioritise the offenses to investigate and identify the source of the suspected security breach for threat hunting.

**IPQS Fraud and Risk Scoring** allows the IBM QRadar users to perform Log activity investigation in real time by using the Right-click menu options.


## 2. Download:

Following steps to be followed while downloading the IPQS Fraud and Risk Scoring App.

* Go to IBM Security App Exchange portal and search for IPQS Fraud and Risk Scoring. 
* Select IPQS Fraud and Risk Scoring App for IBM QRadar.
* From the app description page, Click on Download button to get the zip package for installation. 


**Please note that you will need a active IBMid to download the IPQS Fraud and Risk Scoring App for QRadar from IBM Security App Exchange portal.**


## 3. Installation:

Follow the procedures below to install the IPQS Fraud and Risk Scoring App.

* Log in to your IBM QRadar instance.
* Go to the Admin tab and select the Extensions Management.

** Images here..... **

* On the Extensions Management page click on the Add button.

** Images here..... **

* On the pop-up window, Click on Browse and select the downloaded zip installation package. Check Install Immediately and click Add button.

** Images here..... **

* A pop-up window will open which contains the list of all the items which are part of installation package, click on Install button to continue.
* After installation, a pop-up window will open which contains the list of items which are installed.
* Click on Ok button to continue. 
* Now the Installation is completed.

## 4. Configuration
Once the app is installed, you will need to configure the extension as per your requirement. To do so, follow the steps below

* Go to the Admin tab, scroll down to the Apps section, and select “**IPQS Fraud and Risk Scoring**” App, then click on “Configure IPQS Fraud and Risk Scoring App” (OR) you can Go to the IPQS Fraud and Risk Scoring Dashboard, click on “Configure App”.

** Images here..... **

* On the IPQS Fraud and Risk Scoring Configuration page, you will see the following options.

** Images here..... **

* **IPQS Fraud and Risk Scoring API** Key refers to the API key used to authenticate requests to IPQualityScore server. Enter the API key provided to you by IPQualityScore. If you do not have API Key, please register [here](https://www.ipqualityscore.com/create-account/qradar)

** Images here..... **

* **Enable Proxy** this option is used to define Proxy settings if you desire to Configure Proxy settings to be used by IPQS Fraud and Risk Scoring App to connect with IpqualityScore Server. When you check this option you will see the section to provide Proxy Settings.
    * Proxy Type: Http/HTTPS
    * Proxy IP/Hostname: Give a Valid IP/Hostname
    * Proxy Port: Port number to connect to
    
** Images here..... **

*  If the Proxy server requires authentication, specify a username and password to connect the proxy server that requires authentication.

## 5. Automated Threat Hunting

IPQS Fraud and Risk Scoring App enables the IBM QRadar users to view the IP Address, Email Address, Domain, URL and Phone Number Reputation data in the Offense summary page for the Offense Sources of type Domain/IP Address/Email/URL/Phone. 


To view the IPQS Fraud and Risk Scoring Threat Lookup results on the Offense Summary Page, Go to “Offenses” tab from the menu options.

In order to investigate, Double-click any Offense, where Offense Source is either Domain/IP Address/Email/URL/Phone, You will see the IPQS Fraud and Risk Scoring Reputation data in the tabular format.

* **Domain Reputation Data**:
* **IP Address Reputation Data**:
* **Email Address Reputation Data**:
* **URL Reputation Data**:
* **Phone Number Reputation Data**:


## 6. Manual Threat Hunting:
### Log Activity Investigation:
IPQS Fraud and Risk Scoring App enables the IBM QRadar users to perform Log activity investigation with Right-click menu options. When you right-click on Domain/IP Address/Email/URL/Phone fields in the log viewer or event viewer you will see “IPQS Fraud and Risk Scoring Lookup” option, when you click it, this will open a pop-up windown which will contain the reutation data for the selected Domain/IP Address/Email/URL/Phone field.
** Images here..... **

### Threat Lookup via Dashboard:
IPQS Fraud and Risk Scoring App enables the IBM QRadar users to do Threat Lookup for user provided text irrespective of Log activity (or) offense Sources.

The next step is, go to “IPQS Fraud and Risk Scoring Dashboard”, in the dashboard page select the required type from the dropdown and provide the desired value and click on "Go". This will fetch the reputation data for the provided value and displays it in the tabular format below.

** Images here..... **
