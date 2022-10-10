---
title: Speediness
subtitle: Check your internet speed
date: 2021-11-23
platforms:
  - macOS
appStoreId: 1596706466
---

<br>

### Frequently Asked Questions {#faq}

#### I have a feature request, bug report, or some feedback

[Send it here.](https://sindresorhus.com/feedback?product=Speediness&referrer=Website-FAQ)

#### Why does it show different result from other tools? {#different-result}

By default, tests are run in parallel to better reflect real-world situations (video chat and voice calls). Because of this, speeds may differ from other tools. You can change this in the preferences.

#### How does it compare to Speedtest by Ookla? {#ookla}

The Speedtest app uses a nearby server, which means the speed does not reflect real-world usage — it shows the most optimal scenario. Its requests are also often prioritized by ISPs, which skews the numbers even more. Speediness also looks more like a proper macOS app and it has support for Shortcuts.

#### How does it compare to fast.com? {#fast}

The problem with fast.com is that it's run by Netflix, and Netflix's servers are often prioritized (and sometimes throttled), meaning you won't always get a realistic value. It pretty much gives you your speed for watching Netflix.

#### What does the responsiveness (RPM) value mean?

It's a measurement called Round-trips Per Minute (RPM) — the number of sequential round-trips a network can do in one minute under normal working conditions.

[Read more](https://support.apple.com/en-gb/HT212313)

#### What does the ping value mean?

It's a measurement of the round-trip time for messages sent from the originating host to a destination computer that are echoed back to the source. `ms` is the symbol for milliseconds.

[Read more](https://xtrium.com/what-is-a-good-ping-speed/)

#### Why should I trust the results?

The app makes use of the built-in [`networkQuality` command-line tool](https://support.apple.com/en-gb/HT212313) under the hood, which is provided by Apple.

#### Can it show the current speed live as it calculates it?

This is not possible as it's not provided by the macOS tool Speediness uses to get the speed.

I have sent a [feature request to Apple](https://github.com/feedback-assistant/reports/issues/346) about it and I encourage you [to do the same](https://www.apple.com/feedback/macos.html). Feel free to copy-paste my report.

#### How can I run it from the menu bar?

Open the Shortcuts app, create a new shortcut, and then drag the “Get Internet Speed” action into the shortcut editor. Enable the “Pin in Menu Bar” shortcut setting. You can now run speed tests directly from the Shortcuts icon in the menu bar.

#### How can I run the speed test automatically every hour? {#scheduled}

Open the Shortcuts app, create a new shortcut, and then drag the “Get Internet Speed” action into the shortcut editor. You may want to enable the “Add to History” action setting. [Get the Shortery app](https://apps.apple.com/no/app/shortery/id1594183810?mt=12) and set it to run this shortcut every hour or at an interval of your choosing. (The Shortery app is only needed this year. It's almost certain that Apple will introduce automation for Shortcuts in macOS 13)

#### Can you add support for iOS? {#ios}

This is unfortunately not possible at this time as the app relies on the built-in [`networkQuality` command-line tool](https://support.apple.com/en-gb/HT212313), which does not exist on iOS. Someone would have to implement the [“Responsiveness under Working Conditions” RFC](https://github.com/network-quality/draft-ietf-ippm-responsiveness/blob/master/draft-ietf-ippm-responsiveness.txt) in Swift. [Reference implementation in Go.](https://github.com/network-quality/goresponsiveness) Let me know if you end up making a Swift package for this.

#### Is the app native?

Yes, it's native and written in Swift and SwiftUI.

#### Why is this free without ads?

I just enjoy making Mac apps. Consider leaving a nice review on the App Store.

#### Where can I find the changelog?

Go [here](https://apps.apple.com/app/id1596706466) and click “Version History”.

#### Can you localize the app into my language?

I don't have any immediate plans to localize the app.

<br>

### Non-App Store version

A special version for users that cannot access the App Store. It won't receive updates.

[Download](https://dsc.cloud/sindresorhus/Speediness-1.4.2-1661934168) *(1.4.2)*

*Requires macOS 12 or later*
