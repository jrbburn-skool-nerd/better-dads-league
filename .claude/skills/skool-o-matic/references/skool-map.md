# The Skool map — what lives where, and what to trust

This is field knowledge from years of building tools on Skool. Skool has no public API for this kind of work; everything here is what a logged-in operator can SEE in their browser. That's the whole game: if an admin can see it on a page, a tool can be built on it. If they can't, be suspicious of any plan that claims otherwise.

Skool updates its design from time to time. Treat this map as "what to look for," not "exactly where the pixel is" — always read the actual page in front of you, and if something described here isn't where expected, look around before declaring it gone.

## The surfaces

**Community feed (the home tab).** Posts with author, category, likes, comment counts, pinned posts at top. Good for: what's getting engagement, who's contributing, which categories are alive or dead. Category names are set by the owner and get renamed or deleted over time — never assume last month's category list still holds.

**Members page.** The roster. For each member (visible to admins): name, profile picture, level, a short bio line, join info, and an activity hint (things like "Online now" or "Active 3d ago"). There are filters/tabs for admins vs members and (for admins) churned/banned views. This page is the backbone of most member-attention tools. It paginates — for large communities, decide with the operator whether you need everyone or just a useful slice (recently joined, currently displayed, etc.) before grinding through hundreds of pages.

**Member profile (click a member).** Fuller picture: bio, level and points toward next level, contribution stats, sometimes location/socials, their recent activity. Use it to confirm before flagging someone — a member who looks quiet on the roster sometimes turns out to be active in comments.

**Leaderboards page.** 7-day, 30-day, and all-time rankings by points (points come from likes on posts and comments — so leaderboards measure *appreciated contribution*, not raw posting). Also shows members close to leveling up. Good for: celebration tools, spotting rising members, catching a formerly-top member who's vanished from the 30-day board.

**Levels.** Every member has a level from 1 to 9. Level 1 = hasn't earned points yet (or barely). Level is the single most useful one-glance signal of how invested a member has been over their lifetime. New-and-quiet Level 1s and long-time Level 4s going silent are different problems — treat them differently.

**Membership requests (admin only, for private communities).** Pending joins, each with the person's answers to the community's joining questions. Good for: a triage assistant that summarizes answers and drafts (never sends) a personal welcome.

**Calendar.** Community events with RSVP counts. Good for: pre-event nudge lists ("who RSVPed"), post-event follow-up drafts.

**Classroom.** Courses and module structure; per-member progress is limited from the operator's side. Don't promise granular "who finished lesson 3" tooling without checking what their plan actually shows on screen.

**DMs.** Exist, work one-at-a-time. Tools may DRAFT messages; a human sends each one by hand. (See guardrails — this is a hard line.)

**Admin settings → member export.** Skool lets owners export a member CSV (names, emails, join dates, and more). This is the best route for whole-community analysis, dashboards, and anything involving hundreds of members — one download beats fifty page loads. If a wish is really an analysis wish, steer here.

## What to trust, and how much

- **Trust what's rendered on screen** for the community you're standing in. Read the visible page. Don't dig into hidden page data or network responses — it's not built for you, it changes without notice, and it can mix in data from other communities. Tools built on visible content survive redesigns far better.
- **Confirm the community before every gathering pass.** The community name is on the page. People run multiple communities, and the same member can exist in several — never mix rosters. A tool that reports Community A's quiet members while looking at Community B is worse than no tool.
- **Activity hints are coarse.** "Active 2d ago" means presence anywhere on Skool-things-they-do, not "read your post." Use activity for *finding* people, and say "hasn't been around in about two weeks" rather than false-precision claims.
- **Points/leaderboards measure likes received.** A member can be a devoted quiet reader and show zero points. Never let a tool label low-point members "not engaged" out loud to the operator without this caveat.
- **Counts drift.** Member counts and like counts are fine for direction, not for accounting. Round in your language ("about 40").

## What Skool does NOT show (common wishes to redirect)

- **Who read or saw a post** — no read receipts. Redirect to likes/comments as the visible proxy.
- **Who is about to cancel** — no churn signal. Redirect to the earliest visible sign: activity going quiet, especially in previously-active members.
- **Time-on-site, visit history, analytics per member** — not exposed. Redirect to level + activity hint + leaderboard movement.
- **Email open/click behavior** — Skool's own notifications are a black box. Redirect to in-community signals.

When redirecting, always name the wish, name the gap, and offer the nearest real thing in the same breath.
