# Privacy Policy — Batter Up Fantasy

**Last updated:** May 12, 2026

Batter Up Fantasy ("the App") is an iOS application that tracks Major League Baseball starting lineups for players you roster in your Yahoo Fantasy Baseball leagues. This privacy policy explains what data we collect, why we collect it, and what we do with it.

## What we collect

The App collects only what is necessary to deliver its core functionality:

1. **Your Yahoo Fantasy authorization** — When you sign in, Yahoo issues us an OAuth access token and refresh token. These tokens let the App read your Yahoo Fantasy Baseball rosters on your behalf. **We never see your Yahoo username or password** — you enter those directly on Yahoo's login page. We store these tokens server-side (in Cloudflare KV) so we can refresh your roster without requiring you to sign in repeatedly.

2. **A push notification device token** — When you grant the App permission to send notifications, Apple issues a unique device token. We store this token server-side and use it solely to deliver lineup-related push notifications to your iPhone via Apple Push Notification service (APNs).

3. **Your Yahoo profile identifier (GUID) and nickname** — Returned by Yahoo at sign-in time, used to look up your rosters and personalize the in-app greeting.

4. **Your ESPN Fantasy session cookies** — If you choose to connect ESPN Fantasy, your ESPN session cookies (SWID and espn_s2) are captured from the in-app WebView after you sign in on ESPN.com. **We never see your ESPN password** — you enter it directly on ESPN's login page. We store these cookies server-side (in Cloudflare KV) to read your ESPN fantasy rosters on your behalf.

## What we do NOT collect

- We do not collect your name, email address, phone number, or any other contact information beyond what Yahoo's nickname field provides.
- We do not collect location data, contacts, photos, microphone audio, health data, or financial information.
- We do not use analytics, advertising, or any third-party tracking SDKs.
- We do not collect crash reports or telemetry.

## How your data is used

Your Yahoo tokens are used only to:
- Fetch the leagues and teams you manage
- Fetch the current rosters on those teams
- Cross-reference those rosters against MLB's free public StatsAPI to detect when your players are in (or out of) the official starting lineups for each day's games

Your device token is used only to deliver push notifications about your rostered players. Notifications are triggered server-side every five minutes during MLB lineup-posting hours.

## Who we share data with

**Nobody.** We do not sell, rent, or share your data with third parties. There are no advertisers, no analytics providers, no data brokers involved.

The App communicates with four services to function:
- **Yahoo Fantasy Sports API** (api.login.yahoo.com and fantasysports.yahooapis.com) — for OAuth and roster data
- - **ESPN Fantasy API** (fan.api.espn.com and lm-api-reads.fantasy.espn.com) — for reading your fantasy rosters if you've connected ESPN
- **MLB StatsAPI** (statsapi.mlb.com) — for public game schedules, lineups, and player stats; no personal data is sent
- **Apple Push Notification service** (api.push.apple.com) — for delivering notifications

## Data retention and deletion

Your Yahoo tokens and device token are retained for as long as you use the App. If you want your data deleted, you can:

1. **Delete your account in-app** Settings → Account → Delete account) — this immediately removes all server-side data (Yahoo tokens, device tokens, cached roster data) and signs you out. The action is irreversible.
2. **Email us** at the support address below and request full deletion of your server-side records. We will delete your Yahoo tokens, your Yahoo GUID, and any registered device tokens within seven (7) days of the request.
3. **Revoke access from Yahoo directly** — visit https://login.yahoo.com/account/preferences/apps to remove Batter Up Fantasy's access at any time. This immediately invalidates our stored tokens.
4. **Revoke access from ESPN directly** — sign out of espn.com in any browser. This invalidates the session cookies we stored.

## Children

The App is not directed to children under 13 and does not knowingly collect data from anyone under that age.

## Changes to this policy

If we update this policy, we will revise the "Last updated" date at the top. Material changes will be noted in the App's release notes.

## Contact

Questions or data-deletion requests:
**Email:** alexander.arnowitz@gmail.com
