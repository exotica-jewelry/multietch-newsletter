# Zoho settings for a standard email

This guides you through creating an email campaign from scratch; if instead
you've copied or cloned an existing campaign, some of the following will already
be set up.

* The merge tag for the first name is `$[FNAME|Multi-Etch User|Multi-Etch User]$`
* Campaign (internal) title should be in the form `2022-01-31 Newsletter`
* Place the campaign in the appropriate folder; for newsletters it's
`Newsletters`.
* Copy subject from `title.hbs`.
* Copy preheader from `preview.hbs`.
* Sender (same for all) is `Chris, Multi-Etch Answer Man`
* From address is `info@`
* Click "Show reply-to address details" and choose "Reply Tracking".
* If offered, check the box for including a customer's email in the "To" field.
* Recipients will be the appropriate mailing list for the email. If this is a
newsletter **be sure to exclude** people in the "Welcome" email series.
* To create the content, choose "HTML Editor" (on the bottom row of choices). If
content already exists (from cloning an existing campaign), edit the content,
select everything (ctrl-A) in the editor and delete it.
* Choose the image icon in the toolbar and upload all necessary images. You can
leave all the settings as default. The images will appear in the area below;
leave them there and we'll take care of them in the next step.
* Choose the `</>` icon in the toolbar. Under some standard HTML you'll see the
code for the images you inserted. Find the URL for each image, which will start
with `https://campaign-image.com/zohocampaigns/`, and copy each one into the
appropriate place in the MJML files. Rebuild the `index.html` file. (Whew!)
* Now copy Premail's generated `index.html` into the code window you've already
opened, replacing everything that's there.
* At the top, click "Save Changes" and then "Preview and Test".
* Above the content display, click "Add Preheader". Copy the text from
`preview.mjml` and paste it here. (Why Zoho makes us do this twice we do not
know). You may have to remove line-breaks.
* If the content-editing screen doesn't close automatically, click "Save and
Next".
* Zoho sometimes displays an error message here about custom font stylesheets
not being loaded. Re-saving (or reloading in the browser) of the email seems to
make this go away -- and fonts are loaded just fine -- so this seems to be a
Zoho bug.
* To the right of the content preview, click "Edit plain text".
* Zoho will have auto-generated a plain-text version of the newsletter. Copy and
paste Premail's plain-text version, replacing everything that's there. You may
still need to do a little hand-editing, especially around links, buttons, and
the bottom navigation/footer.
* To the right of the content preview, make sure the "Header Footer Theme"
is set to "None (No Header and Footer)". If it's not, click "change theme" to
set it correctly. We include the header and footer ourselves.
* If you want to set up custom scoring for customers who click links, at the
bottom of the screen, click "Show advanced options" and then create
campaign-specific scoring rules.
* Again to the right of the content preview, click "Send test email" and send
yourself both HTML and plain text versions. You can send any number of these,
for instance if you want to preview in different email accounts on different
devices.
* Double-check the plain-text email; sometimes the first time you enter the text
version it doesn't "take" and you'll need to edit it again. This seems to be a
bug in Zoho.
* Finally, at the top of the screen you will probably need to send the campaign
to Zoho to review -- this usually only takes a few moments. Take a break.
* Once approved, schedule the campaign for "recipients' optimal open time."
