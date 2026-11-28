# Part C — privacy page check (https://atrest.app/privacy.html)

Opened 2026-11-28. Every quote was checked by script as an exact substring of the page text. The developer's name and email are left out on purpose.

1. Loads: yes, HTTP 200.
2. Who runs it: "an individual developer in Belgium" (Belgium).
3. Anthropic / AWS: both named. "made by Anthropic and run for us by Amazon Web Services, which writes the reply. Both are in the EU."
4. AI chat data: "Our server keeps none of your messages, and we've set the AI to keep nothing either. Your conversation is stored only on your phone." Reported replies are kept: "kept on our server for a short time (at most 85 days)".
5. Voice notes: "the app uses Apple's speech recognition with on-device recognition required, so the audio is processed by your phone and not sent to Apple". Where the phone can't do that: "the app produces no transcript rather than sending the recording away instead"
6. Analytics and third-party code: "No analytics, no usage tracking, no advertising, no advertising identifier." "No crash or error reporting from inside the app." "No third-party code of any kind."
7. Minimum age: "Atrest is rated 18+ on both stores."
8. Last updated: "Last updated 24 November 2026"
9. Gaps against the claim "Everything stays on your phone. No account, no analytics, no third-party code. Chat goes through our server to an AI, both in the EU, and neither keeps it. Voice notes are transcribed on the phone and never sent anywhere."
   - "Everything stays on your phone": the page lists exceptions. Reported replies on the server up to 85 days; iPhone backups ("the app's data can be included in that backup"); emails to the developer.
   - "Neither keeps it": true for chat messages. Reported replies are kept up to 85 days.
   - "Voice notes … never sent anywhere": true for transcription. Voice notes are part of the app data that backups can include.
   - Consistent with the app, but add context: Apple and Google may show crash data from their own systems ("Apple may also show me anonymised crash reports"), and the web host logs visits ("Like every website, the service hosting these pages records the requests it receives, which includes your IP address.").
   - The page also covers Android; the claim is about iPhone.
