# Nearby Share web companion

This static site is a GitHub Pages-ready connection launcher. It asks for the
address displayed by a phone running Nearby Share, then opens that phone's
local transfer page. Files and messages travel directly over the local Wi-Fi
or phone hotspot; GitHub Pages does not relay or store them.

The phone must be running Nearby Share with **Start sharing** enabled. Enter
the phone's full address, such as `http://192.168.1.12:8082`, and enter the
temporary PIN on the page served by the phone.

## Publish with GitHub Pages

Copy the contents of this folder into the root of a GitHub repository, push it
to the `main` branch, then select **Settings → Pages → Deploy from a branch →
main → /(root)**. GitHub Pages will provide the public launcher URL.

The phone address is opened as a top-level page rather than fetched from this
HTTPS site. This avoids browser mixed-content restrictions on requests from a
hosted HTTPS page to a private HTTP address.

## Local-network requirement

Both devices must be on the same Wi-Fi or hotspot. This static website is not a
relay and cannot connect devices on separate networks. Keep the PIN private and
stop sharing when finished.
