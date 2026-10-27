# Troubleshooting

## Wireshark will not start
Confirm it is installed in the Linux lab environment and review any terminal error. Follow your administrator's guidance for capture permissions.

## Loopback interface not visible
The source lab says it is often named `lo`. Select the correct loopback interface for your system.

## Telnet or SSH connection refused
The local service may not be running or installed. The supplied lab assumes both services are available but does not give installation steps. Follow instructor-provided setup guidance. Do not expose Telnet to an untrusted network.

## No packets appear
- Start capture on loopback before connecting to `localhost`.
- Generate traffic while capture is running.
- Stop and inspect the correct capture.
- Temporarily clear the display filter to check whether packets were captured.

## Filter shows no results
Use the exact filters `telnet` and `ssh`, and confirm the corresponding session occurred during the capture.

## Privacy
Review screenshots and notes for credentials, tokens, private addresses, hostnames, and other sensitive information. Do not publish raw packet captures.
