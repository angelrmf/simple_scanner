# simple_scanner

A lightweight Python-based TCP port scanner designed to help you quickly check which ports are open on a target host. The project is intentionally simple and modular, making it easy to extend with additional scanning features.

## Features

- Scan a target by hostname or IP address
- Specify a custom port range
- Detect open TCP ports using Python's `socket` library
- Simple, readable code for easy experimentation and upgrades

## Project structure

```text
simple_scanner/
├── README.md
└── scanner_code/
    └── scanner.py
```

## Usage

From the repository root, run:

```bash
python scanner_code/scanner.py
```

You will be prompted for:

- Target (IP or hostname)
- Starting port
- Ending port

Example:

```text
Enter target (IP or hostname): example.com
Start port: 20
End port: 100
```

The script will resolve the hostname, scan the selected port range, and print any open ports.

## Example output

```text
Scanning example.com (93.184.216.34) from port 20 to 100...
Port 22 is OPEN
Port 80 is OPEN
Port 443 is OPEN
Scan finished.
```

## Important note

Only scan systems you own or have explicit authorization to test. Unauthorized scanning may be illegal or violate service policies.

## Planned improvements

- More advanced vulnerability scanning inspired by common network enumeration tools
- Additional scanning options and output formatting
- Potential GUI or web-based interface in the future
