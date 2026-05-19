# Uzuri case studies

## About Project

    Uzuri is a SwiftUI social app case study set that highlights how the team built reliable core systems across authentication, real-time feeds and map-based groups, messaging/media handling, moderation and safety, subscription monetization with RevenueCat, and deep-link push notifications. The write-up focuses on practical engineering choices—state management, service-layer boundaries, coalesced reloads, storage/policy alignment, and entitlement consistency—and emphasizes measurable outcomes (to be filled with real metrics) plus lessons learned for building scalable, low-friction mobile social experiences.

## Technology Stack
    - Platform: iOS
    - Language/UI: Swift + SwiftUI
    - Backend/Data: Supabase (database, auth, realtime, storage)
    - Authentication: Email/session auth + Google OAuth
    - Realtime: Supabase Realtime subscriptions
    - Payments/Subscriptions: RevenueCat + App Store billing
    - Notifications: APNs push notifications + deep linking
    - Media: Image/video upload pipeline with cloud storage and caching

## The client

    The client is a mobile-first social product team building Uzuri, an iOS app focused on community discovery, map-based group interaction, and creator-led engagement. Their audience expects a fast, intuitive experience with reliable login, real-time feed and chat behavior, rich media sharing, safe community interactions, and seamless premium upgrades without friction.

## The Solution

- **Authentication & Session Management**: Implemented app-shell-driven auth state handling with Google OAuth support and persistent session continuity.
- **Realtime Social Core**: Built typed Supabase service layers for feed, profiles, follows, and reactions with controlled realtime subscriptions.
- **Map-Based Group Experience**: Added map-first group discovery with synchronized group chat state and debounced notification-triggered reloads.
- **Messaging & Media Pipeline**: Structured upload, storage, and cache services to support reliable text, image, and video sharing on mobile networks.
- **Trust & Safety Workflows**: Integrated reporting and moderation-aligned client flows to support abuse handling and safer community interactions.
- **Premium Monetization**: Centralized RevenueCat entitlement logic for consistent premium access, paywall flow, and purchase restoration.
- **Push & Deep Link Routing**: Standardized push payload parsing and deferred routing logic to land users on the correct destination screen.

## The results

- Improved sign-in reliability and reduced user drop-off during authentication and session re-entry.
- Delivered a faster, more consistent social experience across feed refreshes, reactions, and map-based group interactions.
- Increased media delivery reliability with stronger upload handling and clearer storage/service boundaries.
- Strengthened user trust through streamlined reporting paths and moderation-ready data flows.
- Reduced premium-access friction by unifying entitlement checks and purchase restore behavior.
- Improved re-engagement quality by routing notification opens to the correct in-app destination.
