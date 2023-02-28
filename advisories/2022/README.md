# PAX Paydroid Vulnerabilities 
This advisory shows the results of a vulnerability research which was conducted on PayDroid_7.1.1_Virgo_V04.3.26T1_20210419 running on the [A930 terminal](https://www.pax.com.cn/androidsmartpos/A930). As a result of this research 4 vulnerabilities were identified (CVE-2022-26579, CVE-2022-26580, CVE-2022-26581, CVE-2022-26582). 

The imapct of those vulnerabilities varies between unauthorized command exectution, privilege escalation and signature check bypass. An attacker who is able to chain some of those vulnerabilities is able to gain RCE as root and install unsigned applications (ex: credit card sniffer) on a production mode POS.

## Exploit Chain Showcase
https://user-images.githubusercontent.com/45386823/221898164-dc192857-2611-4285-bbe6-651f7d6febc1.mp4

## Vulnerabilities
* [CVE-2022-26579](CVEs/CVE-2022-26579.md): Application Signature Verification Bypass
* [CVE-2022-26580](CVEs/CVE-2022-26580.md): Command Injection in ADB Daemon
* [CVE-2022-26581](CVEs/CVE-2022-26581.md): Mulitple Unauthorized Backdoor Functionalities in ADB Daemon
* [CVE-2022-26582](CVEs/CVE-2022-26582.md): Privilege Escalation Through Argument Injection in Systool Client

## Affected Systems
These vulnerabilities were discovered on PAX A930 running PayDroid_7.1.1_Virgo_V04.3.26T1_20210419. However, they may affect other terminals and versions. Please refer to PAX Technology for clarification on vulnerable terminals and/or versions and their respective patched version.

## Responsible Disclosure Timeline
* Discovery: November 01, 2021
* Vendor Meeting: November 17, 2021
* Patching: November 25, 2021 - January 09, 2022
* Disclosure: December 12, 2022

## Acknowledgement
Saif Aziz ([@wr3nchsr](http://twitter.com/wr3nchsr)) of CyShield

## Disclaimer
CYSHIELD FOR TECHNOLOGY S.A.E (CYSHIELD) are keen to share our expertise widely and to enrich public knowledge, through disseminating cyber security culture awareness. CYSHEILD relies on information provided by the vendor / product manufacturer when listing fixed versions, products or releases. CYSHIELD does not verify this contained information, except otherwise when specifically stipulated in the advisory text and contractually required or explicitly agreed in a written form by the vendor / product manufacturer to undertake as such. Unconfirmed vendor / product manufacturer fixes might be ineffective, incomplete, inaccurate or easy to bypass and it is the vendor’s / product manufacturer's liability to ensure all the discovered vulnerabilities found by CYSHIELD are resolved properly. CYSHIELD accepts zero liability, financial or otherwise, from any material and consequential losses, loss of life or reputational loss arising from or as a result of misuse of the information or code contained or mentioned in its advisories. It is the vendor's / product manufacturer’s liability not CYSHIELD to ensure their products' security before, during and after release to market.
