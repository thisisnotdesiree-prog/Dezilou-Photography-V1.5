DEZILOU PHOTOGRAPHY — WEBSITE MAINTENANCE GUIDE
================================================

This guide is for making small updates without rebuilding the website. You can do the edits in GitHub's website once the site is published. Keep a copy of this ZIP as your backup.

FIRST: HOW THE WEBSITE IS ORGANIZED
-----------------------------------
index.html     Homepage
portfolio.html Portfolio film-roll gallery
booking.html   Rates & Booking page and booking form
about.html     About page text and layout
inquire.html   General contact page and inquiry form
style.css      Shared colours, fonts, spacing, and overall design
images/        Website photographs

To preview locally, extract the ZIP first. Keep all files and the images folder together, then double-click index.html. Do not open index.html from inside the ZIP preview.

A. ADD A PHOTOGRAPH TO THE PORTFOLIO
------------------------------------
1. Prepare the photo as a JPG or WebP if possible. Use a short filename with no spaces, for example: couple-sunset.jpg.
2. In your GitHub repository, open the images folder. Choose Add file → Upload files and upload the photo.
3. Open portfolio.html and choose the pencil icon to edit it.
4. Search for the comment ADD NEW PHOTOS. The photo cards are immediately after it. Copy one complete card, from <button class="frame" to its matching </button>, and paste it before the existing photo cards end / before the gallery's closing container.
5. In the copied card, replace both image paths with your exact new filename. For example, change images/frame-08.jpg to images/couple-sunset.jpg. Also update the alt description, caption if present, and frame number so they match the new image.
6. Save by choosing Commit changes. Wait a short time, then refresh the live portfolio page.

Important: Copying a complete existing card preserves the film-strip styling and enlarge-on-click feature. Make sure the filename capitalization matches exactly. GitHub Pages filenames are case-sensitive.

REPLACE AN EXISTING PORTFOLIO PHOTO
-----------------------------------
The simplest safe method is to upload the replacement photo with a new filename, then change that card's image paths in portfolio.html to the new filename. After checking the live page, you can delete the old image if nothing else uses it. Avoid reusing the same filename for a different image because browsers may keep an old cached copy.

B. CHANGE RATES OR BOOKING DETAILS
----------------------------------
1. Open booking.html in GitHub and choose the pencil icon.
2. Find the wording you want to change, such as a session heading, price, package detail, or explanatory paragraph. Edit only that text.
3. Leave the form's technical parts alone unless you specifically intend to change how submissions work. In particular, preserve the form action URL https://formspree.io/f/mrpplzlv, the form field names, and the surrounding <form> and </form> tags.
4. Commit changes, then check the live Rates & Booking page and submit a test using your own email address if you changed the form.

C. CHANGE THE ABOUT PAGE
------------------------
1. Open about.html and choose the pencil icon.
2. Find the existing biography paragraphs and replace only the words between the paragraph tags. Keep the existing <p> and </p> tags around each paragraph.
3. To add a paragraph, copy an existing paragraph element and replace its text. Avoid deleting nearby layout or navigation tags.
4. Commit changes and check the live About page.

D. CHANGE OR REPLACE PHOTOGRAPHS ON OTHER PAGES
------------------------------------------------
The homepage image is currently images/hero-photo.jpg. To replace it, upload a new image into images/ and update the matching image path in index.html. The About page may also refer to image files; update only the relevant image path if replacing one.

E. PUBLISHING CHANGES WITH GITHUB
---------------------------------
1. Open the correct file or folder in your repository.
2. Edit text with the pencil icon, or use Add file → Upload files for new images.
3. Select Commit changes and confirm the commit if asked.
4. GitHub Pages usually publishes automatically within a few minutes. Open the live site and refresh it. If an old photo still appears, try a hard refresh (Ctrl+F5 on Windows) or wait briefly for browser caching to clear.
5. Make one small change at a time, then check the live page before moving on.

F. IMPORTANT THINGS NOT TO CHANGE CASUALLY
------------------------------------------
- Do not rename index.html, portfolio.html, booking.html, about.html, inquire.html, style.css, or the images folder.
- Keep style.css beside the HTML files so the original design loads.
- Keep image files in the images folder and check filenames/capitalization carefully.
- Do not remove navigation, footer, CSS links, script tags, form field names, or Formspree endpoints when editing ordinary text.
- Save a backup copy of the last working website before making larger changes.

FORMS AND EMAIL
---------------
The booking form and the Inquire page use the Formspree endpoint https://formspree.io/f/mrpplzlv. Preserve this endpoint if you want both forms to continue using the same Formspree setup. Form delivery depends on the Formspree account and service, so test after making form-related changes.

The Inquire form checks email formatting and compares the email address with the confirmation field. These checks can catch many typos, but a website cannot guarantee that an email inbox really exists just by checking the address.

CONTACT LINKS
-------------
Email: dezilouphotography@gmail.com
Instagram: https://www.instagram.com/dezilou_photography/

If something looks broken, do not start editing style.css immediately. Restore the last working backup or ask for help with the exact page and change you want to make.
