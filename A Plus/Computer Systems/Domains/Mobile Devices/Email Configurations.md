## Retrieving Mail

- **POP3 (Post Office Protocol 3):**
  - Used for downloading mail to a local mail client.
  - Downloads and optionally deletes from the server.
  - Configuration Information:
    - Name of POP3 server.
    - Username and password.
    - Network ports (Defined by your mail provider).
      - POP3: tcp/110
      - SSL (Secure Socket Layer) settings - POP3S: tcp/995

- **IMAP4 (Internet Message Access Protocol):**
  - Access mail on a central server.
  - Mail is usually stored on the server.
  - Supports folders and server-side searching.
  - Configuration Information:
    - Name of IMAP server.
    - Username and password.
    - Network ports (Defined by your mail provider).
      - IMAP: tcp/143
      - SSL settings - IMAPS: tcp/993

## Sending Email

- **SMTP (Simple Mail Transfer Protocol):**
  - Sends mail from a device to a mail server or between mail servers.
  - Usually sent from a local or trusted device.
  - Authentication usually required.
  - May use different credentials than incoming mail.
  - Port Numbers:
    - SMTP (no authentication, relatively unused): tcp/25
    - SMTP with authentication: tcp/587

## Corporate Email - Microsoft Exchange

- Enterprise email service.
- Not intended for home use.
- More than just email; includes contacts, calendars, and reminders.
- Integrates with mobile device databases.
- Configuration Options:
  - Email, server, domain, username, password.
  - Integrated message encryption with S/MIME (Secure/Multipurpose Internet Mail Extensions).
    - Encrypt and digitally sign.

## Integrated Providers

- **iCloud:**
  - Integrated with Apple Mail.
  - Supports IMAP4.

- **Google (Gmail):**
  - Splits inbox into tabs.
  - Supports IMAP4 and POP3.

- **Exchange Online:**
  - Hosted email service.
  - Supports IMAP4 and POP3.

- **Yahoo Mail:**
  - Supports IMAP4 and POP3.
