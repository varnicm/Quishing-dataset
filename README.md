** URL Security Analyzer

Overview

A simple Python tool to detect suspicious URLs based on:

Unusual TLDs

Random-looking domains

Too many query parameters

Brand names in subdomains

Shortened URLs

Installation

git clone https://github.com/varnicm/Quishing-dataset
cd Quishing-dataset

Usage

Run the script and enter a URL:

python Quishing.ipynb

Example

Safe URL

Input:

https://www.google.com/search?q=python

Output:

URL is normal: https://www.google.com/search?q=python
Number of query parameters: 1

Suspicious URL

Input:

https://secure-login.paypa1.com?auth=abc123&key=secure987&data=xyz789

Output:

Suspicious URL detected!
Phishing brand 'paypal' found in subdomain.
Number of query parameters: 3

Features

 Detects phishing domains

 Identifies suspicious TLDs

 Checks excessive query parameters

 Flags brand misuse in subdomains

 Recognizes URL shorteners

Future Enhancements

 Integrate phishing database checks

 Improve regex for typosquatting

 Web-based analysis tool

Contributing

Fork the repo and submit pull requests!

License

MIT License

Contact

For issues, open a GitHub Issue.

