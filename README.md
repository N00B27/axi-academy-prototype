# Axi Academy, version 2

Open index.html in a browser.

Every page load starts in the visitor view, with Login and no Continue learning banner. Login opens the demo learner homepage with sample saved progress and a Continue learning banner. Log out restores the visitor view.

This is a demonstration switch, not real authentication. Demo user progress is saved under a separate browser storage key. The original website is unchanged.

## Webinars
Visitors can browse the sample schedule and session details. Join Axi Academy opens a demo member account and returns to the selected webinar. Members can register with Join webinar. Registration confirmations appear in Webinar updates and persist in browser storage. Repeated registration is idempotent. Logout hides member registrations.

Dates and instructors are illustrative. This is not real authentication or event registration. Emails, reminders, live meeting links and external schedule changes are not connected.

## Webinar library
Webinars now includes upcoming sessions and past recordings, filtered by topic and session type. Filters persist in the URL and Clear filters resets both. Past sessions open a recording detail view, available to visitors as well as demo members. To enable playback, set `recordingUrl` to an approved MP4 URL on each past webinar record in app.js. No recordings were supplied, so the player area currently shows an honest placeholder. Live registration remains for Academy members only.

## Member courses and cancellation
Visitors see the original six sample courses. Demo members see ten courses, including backtesting, a decision journal, economic events and a risk scenario workshop. Member course links show a login prompt to visitors. This is prototype UI gating, not secure authentication.

Cancel registration is available on registered upcoming webinar cards and detail pages. Cancellation removes the saved registration and its confirmation from updates. Users can rejoin. Course cards now display Free Course.

## Visitor and member overview update
Course tags show only for visitors. Visitors can view lesson previews but cannot start, resume or complete a course or use its quiz. A Join Axi Select prompt leads to clearly labelled demo onboarding. Members retain course controls and quizzes. Their overview replaces the sample lesson with the next upcoming webinar and adds an Axi Select competition information section. Competition dates, rules, eligibility and prizes are intentionally unconfirmed placeholders.
