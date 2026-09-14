# How to update the project website

The site is plain HTML. There is no software to install and no build step. Every file sits in one folder, so anything you add (a report, minutes, a photo) is uploaded to the same place.

- **To edit on GitHub:** open the file in the repository, click the pencil icon, make the change, then click **Commit changes**. The live site updates in about a minute.
- **To edit on your computer:** open the `.html` file in Notepad or VS Code, save it, then upload it to the repository.
- **To preview locally:** double-click `index.html`.

Every spot you will need to change has an HTML comment (`<!-- ... -->`) right next to it showing the exact replacement text. When you edit a page, also update the **Last updated** date at the bottom of that page.

---

## Post a quarterly, draft final, or final report

1. **Make the PDF accessible** (the contract requires it):
   - In Word: *File → Info → Check for Issues → Check Accessibility*. Fix everything until there are no issues.
   - Save as PDF with *Options → Document structure tags for accessibility* turned on.
   - In Adobe Acrobat, run the accessibility checker (*Prepare for accessibility → Check for accessibility*; in older versions *Tools → Accessibility → Full Check*). It must report no issues.
2. **Name the file exactly** as shown and upload it to the repository (all files sit in one folder):
   - `Q1-progress-report.pdf`, `Q2-progress-report.pdf`, `Q3-progress-report.pdf`
   - `draft-final-report.pdf`, `final-report.pdf`
   On GitHub: **Add file → Upload files**, drop the PDF in, then **Commit changes**.
3. In `reports.html`, find the report's row and replace the **Not yet available** badge with the link shown in the comment under it.
4. In `schedule.html`, change that milestone's status badge to **Complete**.
5. Copy the file's web address for the invoice form, for example:
   `https://YOUR-SITE-ADDRESS/Q1-progress-report.pdf`

Also email the Word (.docx) version to hinkleycenter@hinkleycenter.org (cc ttown@ufl.edu and slaux@ufl.edu).

## Post a TAG meeting

1. **Recording:** upload to YouTube (or UNF's video platform) as *Public* or *Unlisted*. Review and correct the captions, since automatic captions alone are not accurate enough.
2. **Minutes and agenda:** upload as accessible PDFs named
   `TAG-1-minutes.pdf` and `TAG-1-agenda.pdf` (use 2 or 3 for later meetings).
   The contract requires the recording and the typed minutes; slides are optional and are not posted.
3. In `meetings.html`, for that meeting:
   - Fill in **Date** and **Format**.
   - Replace each **To be posted** badge with the link in the comment below it (paste the YouTube address for the recording).
   - Change the **Upcoming** badge to **Held**.
4. On the home page (`index.html`), update the **Next meeting** card.
5. In `schedule.html`, change the status to **Complete**.

For the invoice form, the recording URL is the YouTube link. The meeting's page section is `https://YOUR-SITE-ADDRESS/meetings.html#tag-1`.

## Add team headshots

1. Upload square photos (about 400 × 400 pixels) with these names:
   `photo-nickdoost.jpg`, `photo-de-la-cruz.jpg`, `photo-koo.jpg`, `photo-kim.jpg`, `photo-kalasapudi.jpg`, `photo-laddha.jpg`
2. In `team.html`, replace each `<div class="avatar">..initials..</div>` line with the `<img ...>` line in the comment under it.
3. The graduate student's card works the same way (`laddha.jpg`).

## Add news and activity photos

- **News:** in `news.html`, copy the commented pattern at the top of the list and fill it in. Newest items go at the top.
- **Photos:** upload the image, then use the `<figure>` pattern in the comment under **Photos**. Always write `alt` text describing what the photo shows.

The contract asks for photos of investigators and students working on the project throughout the year. Aim for a few each quarter: interviews, meetings, model work, presentations.

## Before posting anything

- [ ] PDFs pass the Acrobat accessibility checker
- [ ] Videos have accurate captions
- [ ] Every image has alt text
- [ ] Link text says what it is ("Download PDF", not "click here")
- [ ] People in photos and recordings agreed to be shown publicly

## Keep the site online

The contract requires the site to stay active for **18 months after the project ends, through February 15, 2029**. Keep the repository public and don't rename it, because the report and recording URLs submitted with invoices must keep working.
