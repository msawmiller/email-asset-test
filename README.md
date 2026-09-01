# Email asset test host

Temporary public host for one email image while it is being tested in real clients.

`youversion_logo_chip.png` is the YouVersion wordmark on an opaque `#f4f4f4` chip. Email needs
the background baked into the pixels because Gmail's dark mode repaints CSS background colours
but cannot alter an image, so a wordmark on a CSS chip goes unreadable there.

This exists only so the asset has a public URL that Gmail's image proxy can fetch during testing.
It is not the permanent home.

## social/

The six footer social glyphs recoloured to the design system's muted grey (#767979), alpha
preserved from the originals. Same reason as the chip: Gmail ignores prefers-color-scheme, so it
renders the light-mode set on a background it has darkened, leaving black glyphs at 1.31:1. Grey
clears 3:1 on every ground - 3.99 light canvas, 4.27 dark canvas, 3.27 Gmail-darkened.
