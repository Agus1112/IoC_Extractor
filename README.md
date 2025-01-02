# IoC_Extractor
This script uses regular expressions to extract various types of indicators of compromise (IoC) from a given text


# IoC Extractor

## Overview
This project is a Python-based tool designed to extract various types of **Indicators of Compromise (IoCs)** from a given text input. It leverages **regular expressions** to identify and categorize IoCs such as IP addresses, hashes, domains, URLs, and MAC addresses.

## Features
- **Extracts IoCs** including:
  - Hashes: MD5, SHA-1, SHA-256
  - IP Addresses: IPv4 and IPv6
  - Domains
  - URLs
  - MAC Addresses
- Simple to use: Just provide a text input, and the script will return the identified IoCs in a structured format.

## Requirements
- Python 3.x

## Installation
1. Clone the repository or download the script file.
2. Ensure you have Python 3.x installed on your system.

## Usage
1. Open a terminal or command prompt.
2. Run the script using the command:
   
   ```bash
   python IoC_Extractor.py
   ```
4. Input the text you want to analyze when prompted.
5. The script will output a dictionary containing the extracted IoCs.

## Example

### Input
```
IPv4: 192.168.1.1
MAC: 00:1A:2B:3C:4D:5E
Hash (MD5): d41d8cd98f00b204e9800998ecf8427e
URL: https://example.com
```

### Output
```json
{
    "ipv4": ["192.168.1.1"],
    "ipv6": [],
    "md5": ["d41d8cd98f00b204e9800998ecf8427e"],
    "sha1": [],
    "sha256": [],
    "domains": ["example.com"],
    "urls": ["https://example.com"],
    "mac_addresses": ["00:1A:2B:3C:4D:5E"]
}
```

## Code Structure
- **`extract_data(text)`**: Main function that processes the input text and extracts IoCs using regular expressions.
- **Regular Expressions**: Defined for each IoC type to ensure accurate pattern matching.

## Contributing
Contributions are welcome! Feel free to open issues or submit pull requests with enhancements or bug fixes.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments
Special thanks to the cybersecurity community for their insights and tools that inspired this project.
