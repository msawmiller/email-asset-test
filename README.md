# Email asset test host

Temporary public host for one email image while it is being tested in real clients.

`youversion_logo_chip.png` is the YouVersion wordmark on an opaque `#f4f4f4` chip. Email needs
the background baked into the pixels because Gmail's dark mode repaints CSS background colours
but cannot alter an image, so a wordmark on a CSS chip goes unreadable there.

This exists only so the asset has a public URL that Gmail's image proxy can fetch during testing.
It is not the permanent home.
