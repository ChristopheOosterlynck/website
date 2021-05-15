+++
categories = ["Xamarin"]
coders = []
date = 2021-05-15T12:00:00Z
description = "Cross platform banking app"
github = []
playstore = "https://play.google.com/store/apps/details?id=be.axa.mobilebanking&hl=nl&gl=US"
image = "https://play-lh.googleusercontent.com/JKCHJWw8_Di3lXtEHGrrfxUvp4Vs2HdaaNJObKnFcqEz80qBjDyUgLAlcC8REMErAIk=s360-rw"
title = "AXA Mobile Banking Service"
type = "post"
[[tech]]
logo = "https://seeklogo.com/images/X/xamarin-logo-217DB116BC-seeklogo.com.png"
name = "Xamarin"
url = "https://dotnet.microsoft.com/apps/xamarin"
[[tech]]
logo = "https://www.mvvmcross.com/assets/img/logo/MvvmCross-logo.png"
name = "MvvmCross"
url = "https://https://www.mvvmcross.com/"

+++

At Flow Pilots I've started out as a developer on the AXA Mobile Banking app. After a while I became the tech lead on this project. I was responsible for 

![Home screen](/axa2.webp "Home screen")
![Investments](/axa4.webp "Investments")

## Functionality

The app started as an app to provide the user with basic daily banking functions. This quickly expanded into more advanced features as consulting and managing investments and requesting loans.

## Technology

The app started out as a Xamarin Android and iOS app with a shared core codebase. To facilitate the code sharing we introduced MvvmCross to the project. The entire app was not refactored to use MvvmCross. MvvmCross was introduced in the existing project and was being used for new features or when existing features required major refactoring because of changes in requirements. This allowed us to quickly introduce this without having to rework the entire app.

The code sharing was really important in this project. We tried to keep as much of the business logic on the backend but even with this effort, a lot of business logic was still present in the app. By implementing this in the shared codebase we only needed to interpret the business/functional analysis only once. This dramatically improved development time for business logic heavy features.

Security was also an important topic for this banking app. Together with AXA I discussed security requirements and made sure these were implemented correctly. The entire authentication/signing flow had to be reworked at a certain point. Together with AXA this was a successful project with little impact for the user by providing a proper migration path.

## Team

The team consisted of 5 developers (including myself). Together with a project manager, designer and functional analysist we were responsible for the development of the Android and iOS app.
