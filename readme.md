## Mail Activities
This Python package contains Mail class to work with emails,
for more information about how to develop your RPA projects with python check https://automatehub.es/

# Mail class

The `Mail` class represents a mail account and provides methods for sending and fetching emails.

## Arguments

- `email`: The email address of the mail account.
- `password`: The password of the mail account.
- `smtp_server`: The SMTP server of the mail account.
- `smtp_port`: The SMTP port of the mail account.
- `imap_server`: The IMAP server of the mail account.
- `imap_port`: The IMAP port of the mail account.

## Attributes

- `username`: The username of the mail account.
- `password`: The password of the mail account.
- `smtp_server`: The SMTP server of the mail account.
- `smtp_port`: The SMTP port of the mail account.
- `imap_server`: The IMAP server of the mail account.
- `imap_port`: The IMAP port of the mail account.

## Methods

### send(send_to, subject, text=None, html=None, files=None)

The `send` method is used to send an email.

#### Arguments

- `send_to`: The email address to send the email to.
- `subject`: The subject of the email.
- `text` (optional): The text content of the email.
- `html` (optional): The HTML content of the email.
- `files` (optional): A list of files to attach to the email.

### fetch(folder, Query)

The `fetch` method is used to fetch a list of emails from the mail box.

#### Arguments

- `folder`: The folder to fetch emails from.
- `Query`: A query object used to filter the emails. More information about the `Query` object can be found [here](https://pypi.org/project/imap-tools/0.16.1/#id2).

### download_attachments

This function is used to download attachments from a mail message.

#### Arguments:

- `mail`: A `MailMessage` object representing the mail from which attachments need to be downloaded.

- `download_folder`: The folder where the attachments will be downloaded to.

- `extension`: (Optional) The extension of the attachments to be downloaded. If specified, only attachments with this extension will be downloaded. If not specified, all attachments will be downloaded.

### More information

For more information about the `Mail` class and the `Query` object, please refer to the [IMAP Tools documentation](https://pypi.org/project/imap-tools/0.16.1/#id2).

