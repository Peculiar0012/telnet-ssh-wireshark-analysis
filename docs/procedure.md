# Lab Procedure

The supplied lab assumes local Telnet and SSH services are available; it does not provide installation/configuration steps for these services.

## Part 1 — Telnet
1. Launch Wireshark from a terminal:
   ```bash
   wireshark &
   ```
2. Select the loopback interface, often `lo`, and start capture.
3. In a second terminal connect:
   ```bash
   telnet localhost
   ```
4. Sign in with a dedicated lab account and run:
   ```bash
   whoami
   ```
5. Stop the capture. Apply Wireshark display filter:
   ```text
   telnet
   ```
6. Select a Telnet packet, right-click, and choose **Follow → TCP Stream**.
7. Record whether application data appears as readable text. Do not record secrets.
8. Close the stream and end the session with:
   ```text
   exit
   ```

## Part 2 — SSH
1. Start a fresh Wireshark capture on loopback.
2. Connect in another terminal:
   ```bash
   ssh localhost
   ```
3. If a host-key confirmation appears, review it and accept only for this controlled lab if appropriate.
4. Authenticate with the dedicated lab account and run:
   ```bash
   whoami
   ```
5. Stop the capture. Apply display filter:
   ```text
   ssh
   ```
6. Locate an SSH packet and choose **Follow → TCP Stream**.
7. Compare it with the Telnet stream and document whether application data is readable as plaintext.

## Part 3 — Document
Complete `observations.md` and `reflection-questions.md`, add your own sanitized screenshots, and complete `evidence/evidence-checklist.md`.

Do not commit raw packet captures or evidence containing credentials.
