+++
categories = ["Android"]
coders = []
date = 2021-05-15T12:00:00Z
description = "Electronic cash register app"
github = []
playstore = "https://play.google.com/store/apps/details?id=be.axa.mobilebanking&hl=nl&gl=US"
image = "/ccv-logo.svg"
title = "CCV SalesPoint"
site = "https://www.ccv.eu/nl/betaaloplossingen/kassasysteem-ccv-salespoint/"
type = "post"
[[tech]]
logo = "/kotlin-logo.svg"
name = "Kotlin"
url = "https://kotlinlang.org/"
[[tech]]
logo = "/realm-logo.svg"
name = "realm"
url = "https://realm.io/"
[[tech]]
logo = "/android-subtitle-logo.png"
name = "Android"
url = "https://www.android.com/"

+++

At CCV Lab I was the mobile lead and one of the projects I worked on was SalesPoint.

![Home screen](/axa2.webp "Home screen")
![Investments](/axa4.webp "Investments")

## Functionality

SalesPoint is a dynamic app which can be a "simple" payment initiation app or a full blown electronic cash register. It can run on Android and iOS devices and integrates with specific hardware (printers, terminals, etc.).

The app is designed to be offline first to allow user to initiate payments in any conditions while making sure no data gets lost.

## Technology

The apps are pure native apps: Objective-C and Swift on iOS and Java and Kotlin on Android. The MVP and MVVM patterns were used for the view logic. Realm database was used for data persistence.

Stability and performance were key quality attributes as this app tends to be open longer (an entire workday) in comparison to "normal" apps. The app also had to run on devices with limited capabilities and needed to be more optimised than on your average Android device available in Western Europe. 
