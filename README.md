# Uzuri case study

## About project

Uzuri is a SwiftUI social app focused on community discovery, map-based group interaction, and creator-led engagement. The product combines reliable authentication, real-time feeds, map-based groups, messaging and media handling, moderation and safety, subscription monetization with RevenueCat, and deep-link push notifications—with emphasis on state management, service-layer boundaries, coalesced reloads, and entitlement consistency.

## Problem

Mobile social apps fail when login is flaky, feeds feel stale, or map and chat state fall out of sync. Uzuri needed a cohesive iOS experience with Supabase-backed realtime data, heavy media on cellular networks, trust-and-safety workflows, and premium access that stays consistent across paywall, purchase, and restore—without users bouncing between broken sessions or wrong screens after a push tap.

## Technology stack

- **Platform:** iOS
- **Language/UI:** Swift + SwiftUI
- **Backend/Data:** Supabase (database, auth, realtime, storage)
- **Authentication:** Email/session auth + Google OAuth
- **Realtime:** Supabase Realtime subscriptions
- **Payments/Subscriptions:** RevenueCat + App Store billing
- **Notifications:** APNs push notifications + deep linking
- **Media:** Image/video upload pipeline with cloud storage and caching

## The client

The client is a mobile-first social product team building Uzuri for users who expect fast discovery, map-based groups, real-time feed and chat, rich media sharing, safe community interactions, and seamless premium upgrades.

## The solution

- **Authentication & session management:** App-shell-driven auth with Google OAuth and persistent session continuity.
- **Realtime social core:** Typed Supabase services for feed, profiles, follows, and reactions with controlled realtime subscriptions.
- **Map-based groups:** Map-first discovery with synchronized group chat and debounced notification-triggered reloads.
- **Messaging & media:** Upload, storage, and cache services for reliable text, image, and video on mobile networks.
- **Trust & safety:** Reporting and moderation-aligned client flows for abuse handling.
- **Premium monetization:** Centralized RevenueCat entitlement logic for paywall, access, and restore.
- **Push & deep links:** Standardized payload parsing and deferred routing to the correct screen.

## Result

- Improved sign-in reliability and reduced drop-off during authentication and session re-entry.
- Faster, more consistent social experience across feed refreshes, reactions, and map-based group interactions.
- Higher media delivery reliability with clearer upload and storage boundaries.
- Stronger user trust through streamlined reporting and moderation-ready data flows.
- Reduced premium friction via unified entitlement checks and purchase restore behavior.
- Better re-engagement by routing notification opens to the correct in-app destination.
