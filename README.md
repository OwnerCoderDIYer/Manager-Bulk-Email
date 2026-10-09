Aged Receivables for Manager.io --- Setup and Customisation
This is a community-built HTML extension, tested by its author on
Manager.io version 25.12.21.3153. It is not an official Manager.io
feature. Back up your data and review every prepared email before
sending.
1. Open the extension
Save `manager-aged-receivables-v4.1-community.html` to your computer and
open it in a browser. Keep Manager open and signed in in the same
browser.
2. Set your Manager server URL
Expand Connection settings and enter your Manager server URL.
Examples:
Manager running on the same computer: `http://127.0.0.1:8080`
Manager running on another computer on your network: use that
computer's reachable address and port, for example
`http://192.168.1.25:8080`
Manager hosted on a server or accessed over HTTPS: use the exact
base URL you normally use to access that Manager installation,
including the correct scheme, hostname and port if applicable.
The `127.0.0.1:8080` value in the extension is only a default/example.
`127.0.0.1` means "this computer"; it will not point to a different
computer running Manager. Do not add `/api2` to the end of the base URL.
Your browser must be able to reach that URL, and Manager must permit the
requests the extension makes. If the extension reports a network, CORS
or HTTP error, check the URL and your Manager/API2 configuration.
3. Add your API2 key
In Manager, create or locate an API2 key with the access needed to read
sales invoices. Paste it into API2 key in the extension and select
Save settings & load.
The key is stored in local storage in that browser profile. Do not share
a copy of the extension with your key inserted, and do not post the key
publicly. If you use a shared computer, consider clearing the
extension's browser data when finished.
4. Email template URL (optional)
Usually, leave Sales Invoice email template URL blank. The extension
first tries to use the invoice's native email form and its template. The
optional URL is a fallback for cases where the invoice page has a blank
subject or message.
If you need this fallback, obtain the Sales Invoice email-template URL
from your own Manager installation and enter the full URL. It must be
on the same origin as the Manager server URL above (same scheme,
hostname and port). Do not copy another user's URL: Manager URLs can
contain business-specific information. The exact URL and availability of
this page can vary by Manager version, so this has not been verified for
every installation.
5. Review before sending
Refresh invoices and check that the displayed balances and due dates
look correct.
Select a small number of invoices for the first test.
Prepare the emails and review each recipient, subject, message and
attachment.
Send only after checking everything. The extension is designed for
user-approved bulk sending, not unattended automatic reminders.
Troubleshooting
No invoices load: check the base URL, API2 key, and whether the
key can access sales invoices.
`127.0.0.1` does not work: use the address of the computer or
server actually running Manager. `127.0.0.1` always refers to the
computer running the browser.
Email subject/body is blank: sign in to Manager in the same
browser and try again. If necessary, configure the optional
email-template URL for your own installation.
PDF or email preparation fails: try opening the relevant invoice
in Manager first, then retry with one invoice. Compatibility with
Manager versions other than the tested version is not guaranteed.
