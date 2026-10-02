<div align="center">

# لمّة · Lamma

**Group outings for people who don't have a group yet.**

A bilingual (Arabic-first, RTL) Flutter app for Egypt: discover an outing, book a seat in the group that fits you, pay, and meet your group in a chat before you meet them in person.

![Flutter](https://img.shields.io/badge/Flutter-3.44-02569B?logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-3.12-0175C2?logo=dart&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-Postgres%20·%20RLS%20·%20Realtime-3ECF8E?logo=supabase&logoColor=white)
![Tests](https://img.shields.io/badge/tests-1302%20passing-success)
![Architecture](https://img.shields.io/badge/architecture-Clean%20·%20Cubit-7B1E2B)

</div>

> **بالعربي:** لمّة تطبيق خروجات جماعية في مصر. بتختار خروجة، وتحجز مكانك في اللمّة المناسبة ليك، وتدفع، وتدخل شات المجموعة وتتعرف عليهم قبل ما تقابلهم. التطبيق عربي أولًا (RTL) وفيه إنجليزي كمان، واتبنى بـ Flutter و Supabase على Clean Architecture. وفيه كمان تاب للبادل تلاقي فيه لاعيبة ناقصين فريق.

---

## Demo

<table>
  <tr>
    <td width="320" align="center"><img src="media/highlights.gif" width="300" alt="Lamma highlights"/></td>
    <td>

**▶️ [Watch the full 5-minute walkthrough](media/lamma-demo.mp4)**, recorded on a real Android build against the live backend. Nothing is mocked:

1. **Onboarding and sign-up**: birth date gives the age automatically; governorate and field of study feed ranking
2. **Booking and Paymob checkout**: a declined card comes back as a clear "booking not completed" plus a notification
3. **Search, filters, favorites**: category, all-in price range, date presets, empty state
4. **Paid booking → group chat**: confirmed by the payment webhook, then text, image, ❤️ reaction and a voice note in the group's chat
5. **Notifications and profile**: server-composed notifications, profile edit, photo upload
6. **Padel**: publish a match missing players in three steps. The wallet is topped up by card, a push notification arrives, and 30 EGP is charged
7. **Wallet, dark mode, English, reviews**: balance and history, withdrawal, full LTR English, verified-attendee review

    </td>
  </tr>
</table>

## Screenshots

<table>
  <tr>
    <td align="center"><img src="screenshots/home.png" width="230"/><br/><sub><b>Home</b>: categories, upcoming outings, suggestions</sub></td>
    <td align="center"><img src="screenshots/search-filters.png" width="230"/><br/><sub><b>Search filters</b>: category, all-in price, date, time of day</sub></td>
    <td align="center"><img src="screenshots/search-results.png" width="230"/><br/><sub><b>Results</b> with the group-discount badge</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/outing-details.png" width="230"/><br/><sub><b>Outing details</b>: which groups it's for, single-gender notice</sub></td>
    <td align="center"><img src="screenshots/booking-summary.png" width="230"/><br/><sub><b>Booking</b>: seat count with the group discount applied live</sub></td>
    <td align="center"><img src="screenshots/wallet-top-up.png" width="230"/><br/><sub><b>Payment rails</b>: card, mobile wallet, InstaPay</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/my-bookings.png" width="230"/><br/><sub><b>My bookings</b> with loyalty-points progress</sub></td>
    <td align="center"><img src="screenshots/booking-details.png" width="230"/><br/><sub><b>Booking details</b>: meeting point, price breakdown</sub></td>
    <td align="center"><img src="screenshots/group-chat.png" width="230"/><br/><sub><b>Group chat</b>: reactions, mentions, deleted messages</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/padel-publish.png" width="230"/><br/><sub><b>Padel</b>: publish a match that is missing players</sub></td>
    <td align="center"><img src="screenshots/notifications.png" width="230"/><br/><sub><b>Notifications</b>, server-composed and localized</sub></td>
    <td align="center"><img src="screenshots/wallet.png" width="230"/><br/><sub><b>Lamma Wallet</b>: top-up, withdrawals, refunds</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/profile.png" width="230"/><br/><sub><b>Profile</b></sub></td>
    <td align="center"><img src="screenshots/home-english.png" width="230"/><br/><sub><b>English (LTR)</b>: every string exists in both languages</sub></td>
    <td align="center"><img src="screenshots/search.png" width="230"/><br/><sub><b>Search</b> suggestions by category</sub></td>
  </tr>
</table>

### From the demo run

<table>
  <tr>
    <td align="center"><img src="screenshots/paymob-checkout.png" width="230"/><br/><sub><b>Paymob hosted checkout</b> (test card)</sub></td>
    <td align="center"><img src="screenshots/payment-success.png" width="230"/><br/><sub><b>Booking confirmed</b> by the webhook, not the client</sub></td>
    <td align="center"><img src="screenshots/chat-voice-image.png" width="230"/><br/><sub><b>Group chat</b>: text, image, reaction, voice note</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/chat-reactions.png" width="230"/><br/><sub><b>Message actions</b>: react, reply, info, copy, edit, delete</sub></td>
    <td align="center"><img src="screenshots/padel-details.png" width="230"/><br/><sub><b>Padel</b>: level, players missing, duration</sub></td>
    <td align="center"><img src="screenshots/padel-published.png" width="230"/><br/><sub><b>Match published</b>, with the server's push notification</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/push-notification.png" width="230"/><br/><sub><b>Wallet top-up</b> lands as a push notification</sub></td>
    <td align="center"><img src="screenshots/withdraw.png" width="230"/><br/><sub><b>Withdrawal</b> to InstaPay, mobile wallet or bank</sub></td>
    <td align="center"><img src="screenshots/review.png" width="230"/><br/><sub><b>Reviews</b> from verified attendees, first name only</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/dark-english.png" width="230"/><br/><sub><b>Dark mode + English</b></sub></td>
    <td align="center"><img src="screenshots/profile-photo.png" width="230"/><br/><sub><b>Profile photo</b> uploaded to Supabase Storage</sub></td>
    <td align="center"><img src="screenshots/search-filters-live.png" width="230"/><br/><sub><b>Filters</b> in use</sub></td>
  </tr>
</table>

---

## What it does

| Area | What's in it |
|---|---|
| **Discovery** | Categories, personalised suggestions, search with filters (city, group size, all-in price range, date presets, morning/evening, sort, hide-full) |
| **Groups** | One outing has **many** groups, one per audience (e.g. engineering students, medical students) plus a default. Targeting affects ranking and visibility, **never** who is allowed to book. |
| **Booking** | Party size, per-group *and* per-outing capacity, group discounts, and an all-in price (ticket + fee + 14% tax) that matches at every step |
| **Payments** | Paymob card, mobile-wallet (Vodafone / Orange / Etisalat / WE) and InstaPay rails, an in-app wallet, refunds, withdrawals |
| **Waiting lists** | A full outing or padel match offers you a place in line. When a seat frees up, the next person's turn is protected. If several people race for one seat close to start time, the losers go back to their place in line and get told why. |
| **Cancellation policy** | Refund tiers by notice given. Repeated cancelling costs you booking rights for a period, not your refund. |
| **Group chat** | Realtime via Supabase: voice notes with playback speed, images, replies, @mentions, reactions, edit/delete, message info |
| **Padel** | A fifth tab where players missing a team find matches missing players, filtered by gender, age and skill, and pay per seat |
| **Also** | Reviews, favourites, safety reports & blocking, in-app feedback, push notifications (FCM), light/dark themes, Arabic/English |

---

## Architecture

Clean Architecture per feature, with dependencies pointing inward:

```
lib/features/<feature>/
├── presentation/   pages, widgets, Cubits
├── domain/         entities, repository interfaces, use cases   ← pure Dart, knows nothing about Supabase
└── data/           DTOs, data sources, repository implementations
```

| | |
|---|---|
| State | `flutter_bloc`, Cubits only |
| DI | `get_it`, where each feature registers itself |
| Navigation | `go_router` with auth and profile-completion guards |
| Errors | `Either<Failure, T>` (`fpdart`) through one `NetworkCallHandler` |
| Backend | Supabase: Postgres, Row-Level Security, RPCs, Realtime, Storage, Edge Functions |
| Payments | Paymob, with confirmation only from an HMAC-verified webhook |
| Push | Firebase Cloud Messaging |
| Tests | `flutter_test`, `bloc_test`, `mocktail` |

### The rule that shaped the backend: *the client is never trusted with money or other people's data*

- **Payment confirmation** comes only from the HMAC-verified Paymob webhook (an Edge Function). The app never reports its own success.
- **Capacity** is enforced inside one Postgres function (`create_booking_atomic`). It locks the outing row first, then checks the group's capacity *and* the outing's total, so two people can't take the last seat at once.
- **Seat counts** come from a `SECURITY DEFINER` function. RLS only lets a user read their own bookings, so counting in the client would only ever count yourself.
- **Review eligibility, refunds, waiting-list turns and cancellation limits** are all checked again on the server, so a modified client gets refused there.

---

## By the numbers

| | |
|---|---|
| Feature modules | 14 |
| Dart files | 527 |
| Tests | **1,302 passing** across 144 files |
| SQL migrations | 177 |
| Edge Functions | 7 (payments, webhook, push, …) |
| Localized strings | ~1,300 keys × 2 languages |
| Merged pull requests | 60 |
| CI | format · analyze · test on every PR |

---

## How it was built

**1. Design first.** Every screen was designed in Figma, then built in Flutter against mock data, screen by screen, before any backend existed. That froze the UI contract early and meant the backend work was only "replace the mock".

**2. One feature at a time.** The backend integration followed a written roadmap (F0 → F25). Every feature went through the same loop: *discuss → approve → implement → analyze → test → verify on a device → update the roadmap*. Nothing ran in parallel on shared files.

**3. Verify the live database, never guess it.** Before touching any table, the real schema was queried from the linked Supabase project. The planning docs turned out to be wrong about table names (`outings` was really `activities`, `chat_messages` was really `messages`), and checking first caught that before it became bugs.

**4. Pair-programming with Claude Code.** I built this with Claude Code as a pair programmer. What made that work was the rules around it:
- A `CLAUDE.md` in the repo holds the architecture, the domain facts that are easy to get wrong, and the git rules. Every session starts from the same context.
- Specialised sub-agents (architect, backend, flutter-dev, testing, reviewer) each have a narrow job.
- Nothing leaves the machine without my approval: every commit, push and PR is mine to say yes to. `flutter analyze` is judged by its **exit code**, not by eyeballing warnings.
- Tests have to fail without the fix before they count.

**5. Lessons written down where the next person will read them.** A few that each cost real debugging time:
- Dropping a `UNIQUE` constraint silently broke **four** payment/cancellation functions that depended on it, and they surfaced one at a time. Now: search `pg_proc` for every dependent function first.
- Adding a defaulted parameter to a Postgres function doesn't replace it. It creates an **overload** and leaves the old body live.
- The test suite mocks the database, so it has no RLS and no stored procedures. Anything touching either is verified on a device, because the suite will pass while the app is broken.

---

## Status

Actively developed. The core flows (auth, discovery, booking, payments, bookings, chat, notifications) are built and verified on Android. The newest features (padel, waiting lists, the latest chat additions) are built and tested but not yet fully device-verified. iOS is pending its Google Sign-In client configuration.

The source code is private. I'm happy to walk through it. Reach me at **[sfhmy7124@gmail.com](mailto:sfhmy7124@gmail.com)**.

<div align="center"><sub>Built with Flutter · Supabase · a lot of Arabic RTL edge cases</sub></div>
