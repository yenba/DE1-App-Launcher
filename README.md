# ****Installable DE1 App Launcher****

Hello! I made a thing and figured if I wanted it, maybe others would too! Long story short, I made installable APKs that launch the DE1 Apps. If that interests you, continue reading!

## **Use Case**

I was annoyed that there wasn't a way to directly launch the DE1 App from an actual app and instead you had to use the Androwish created icons. This meant it was a pain to interact with the app from other automations like Tasker. It also meant you couldn't launch the app from various third-party widget programs, and lastly, it was just bugging me that it didn't show up in the app drawer.

## Solution / Instructions

I used Tasker and Tasker App Factory to create installable APKs that launch the DE1 App and the DE1 Cloud Update App. Just install these APK's and you'll have launchable apps in your App Drawer for both the DE1 app and the Cloud Update app. From there, make shortcuts to them on your home screen, use them in automations, etc. Note, this does not actually install either of these applications. You'll need to already have the de1plus folder in place for it to work.

[DE1_App_Launcher.apk](DE1_App_Launcher.apk)

[DE1_Cloud_Update_Launcher.apk](DE1_Cloud_Update_Launcher.apk)

## What It Looks Like

Here's a quick video of what it looks like launching both apps from the App Drawer and then making shortcuts on the home screen. Your tablet may look a bit different than mine, I'm running LineageOS and I've installed Nova Launcher and customized things a bit.

https://user-images.githubusercontent.com/17832515/169674478-6d384e83-b2a4-49c3-b4e6-3e12f27c3957.mp4

## Make It Yourself

The process was fairly simple if you don't trust using my APKs or just want to do it yourself. Just create a new Tasker task for both the DE1 App and the Cloud Update app. All the task needs to do is use the Browse URL task and point to the following paths.

```
### URL to launch de1plus app
androwish:///storage/emulated/0/de1plus/de1plus%2Etcl

### URL to launch cloud updater
androwish:///storage/emulated/0/de1plus/appupdate%2Etcl
```

For better instructions on how to make these tasks, check out the post Spence made. [Launch app and create DE1 icon with Tasker - Decent Diaspora](https://3.basecamp.com/3671212/buckets/7351439/messages/2108700903)

Once you've got that made, you'll want to export the task using App Factory. There are many tutorials on that if you just Google, "Create APK using Tasker App Factory".

## Wrap-up

There may be a better way to do this than through Tasker and App Factory but without much programming knowledge, it was the easiest way to accomplish what I wanted. No guarantees it will work for you but it worked perfectly in my tests! Also, I'm no designer so if you've got an idea for a better-looking icon, feel free to share! Let me know if you've got any questions! Enjoy!
