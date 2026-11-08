# dwarka.richwealth.in

Confidential investor page and registration for the Dwarka coastal resort project discussion
(Mon 9 Nov 2026, 3–5 PM IST, Google Meet).

- `index.html`: the whole page. All text is plain HTML and can be edited directly. No build step.
- `resort.jpg` / `resort-900.jpg`: AI concept image (captioned on the page as not a site photo).
- `apps_script.gs`: registration backend. Setup steps are at the top of the file.
  After deploying it, paste the `/exec` URL into `ENDPOINT` near the end of `index.html`.

Until `ENDPOINT` is set, the form refuses to submit and shows the WhatsApp help number.
The page shows "Registration received" only after the backend confirms the row was saved.

Meeting link workflow: the team checks each sheet row, sends the Meet link on WhatsApp and by
email, and ticks the "Meeting Link Sent?" column.

Deploy: GitHub Pages (same setup as rw-seminar / rw-careers) + `CNAME` = dwarka.richwealth.in,
plus a Hostinger DNS CNAME `dwarka` → jitenmodhwadia.github.io.
