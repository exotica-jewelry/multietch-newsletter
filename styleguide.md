# Style guide for Multi-Etch emails

When developing new designs for Multi-Etch emails, the following style guide
should be used.

* Logo is [hosted on Zoho](https://campaign-image.com/zohocampaigns/multietch_zc_v9_1_722626000001654004.png).
* Brand purple is `#46175b`.
* The current font stack uses
[Google Fonts' Hind](https://fonts.google.com/specimen/Hind), though this could
be changed in a new design. Premail will then append system fonts with emoji
support. Remember that only some email clients will see the custom font.
* In-text links should always be underlined. Exceptions are only for obvious
menu items (i.e. not "in-text"), buttons (see below) or linked images/graphics.
* Buttons should be of the form:
`<mj-button mj-class="button" css-class="button" href="#" title="TITLE">TEXT</mj-button>`
or:
`<mj-button mj-class="button button--ghost" css-class="button button--ghost" href="#" title="TITLE">TEXT</mj-button>`
The CSS classes are necessary for styling of the link elements.
* Link-hover/active/focus states should only be used for enhancement, as not all
email clients will see them.
* Prominent links should appear as buttons, set off by themselves, rather than
(only) links within paragraphs.
* All non-decorative images should have alt text (enforced by Premail).
* Images should be sized at twice their HTML-displayed width, for
high-res/retina display.
* Images should be pleasing at full-width. They can be displayed in columns at
desktop widths, but will still be full-width at smaller screen sizes.
* If images are floated with CSS (as opposed to using MJML columns), it should
be made clear that only some email recipients will see them, and the text/image
layout should be readable even if the image float is disabled.
