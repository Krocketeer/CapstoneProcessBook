---
layout: page
title: Prototyping
nav_exclude: false
nav_order: 9
parent: Design
---
# Prototyping
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}
---

Our ideation phase led us to our final prototype for Dropbox Clip. Outlined below is our process as well as the features of our product and considerations for future steps of the project.

## Goals

The goal and ultimate purpose of prototyping our concept is to present a visual aid to Dropbox and other major stakeholders, such as our professors and department heads. With a visual prototype we can better explain our ideas and provide a more convincing argument of the product.

## Process

From our ideation sketches, we moved into creating mid-fi screens (Figure 4). We started with mid-fi rather than lo-fi or wireframing because a lot of our concepts were based on incorporating Dropbox functionality into the operating systems of phones, tablets, and computers, so it made the most sense to build on top of screenshots, rather than build out wireframes. Figure 4 outlines a few of the assets we created, along with our critique to keep in mind as we move forward in our process.

![Mid-Fi Screens](../images/screens.png)
***Figure 4**: Examples of two Mid-Fi screens for the clipboard being accessed from the shortcut menu on desktop.*

From this mid-fi critique, we developed two more rounds of screens, adding mobile, tablet, and desktop prototypes. By doing multiple rounds of mid-fi prototypes and critique, we were able to refine our designs before focusing on details and making them final. We were also able to work through the high-level concepts of our product as we ran into problems, such as “How can you paste from different applications?” and “Where can users access Clip on their different devices in the most intuitive ways?” By having these discussions as we’re generating our designs, we were easily able to refine our designs and concepts before making anything final.

## User Testing

We completed five rounds of user testing with classmates and peers who were not involved in our project. We gave them a mobile device and a laptop with our figma prototype and asked them to complete the following tasks:

- Copy an image on the phone, paste on the desktop through the shortcut menu
- Copy an image on from the desktop Toolbar Menu, paste on desktop with the Command+V Keyboard command
- Copy and paste on desktop using Drag & Drop
- Download from the Toolbar Menu on desktop
- Paste from the shortcut menu on mobile
  
We asked participants to think aloud while completing these tasks, asking them along the way about their reactions and expectations. This included asking users where they might find certain menus, or how they would expect an interaction to play out before they completed it.

From these user tests, we learned valuable information about our prototype to implement into our final design. Here are a few key insights:

- Drag & drop is the most favored and intuitive interaction for copying and pasting on desktop
- While most people recognized the download icon, the visibility of the icon was low
- Downloading on mobile was very intuitive
- When accessing the mobile clipboard menu, they expected the text “Paste from Dropbox Clip” to paste something, not access the clipboard

## Dropbox Clip

### Overview

As mentioned before, Dropbox Clip is a multi-device clipboard with an expanded capacity. Users are able to copy content on one device and paste it on another, regardless of operating system. The sections below outline the key features and value props of Clip.

#### Cross-Device Functionality and Speed

Currently, if users have the full Apple Ecosystem, they are able to copy an image on their phone and paste it on their computer instantly. However, this is not the case for those without a complete Apple Ecosystem, forcing them to upload items to the cloud or email files to themselves. These solutions take too much time, and we know that Gen-Z students want their files to be transferred between their devices quickly. Clip allows users to copy their items as normal, storing the copy into their Dropbox Clipboard which updates across devices (Figure 5). Since it’s not actually being updated to the cloud, just copied, it doesn’t take the amount of time it would take to upload the entire file. Users can access this clipboard in a variety of ways.

![Cross Device Usage](../images/CrossDeviceUsage.png)
***Figure 5**: (left) Users are able to copy an image from their iPhone like normal. This is put into Dropbox Clip, which can be accessed from any device. (right top) To access the most recent item that has been copied to Dropbox Clip, users can right click to pull up the shortcut menu. (right bottom) After pressing “Paste from Dropbox Clip,” the most recent item that has been copied into Clip is pasted.*

#### Expanded Capacity

The speed and cross device functionality isn’t all: users are able to hold up to six items in their Dropbox Clipboard at a time (Figure 6). If there are six items in the clipboard and they copy a new item, their oldest copy is removed. By expanding the capacity of the clipboard, Clip allows users to recopy items from the past. This is especially useful during project work sessions, knowing you’ll need assets repeatedly but don’t want to have to keep searching for them. 

![Pop up menu](../images/popup.png)
***Figure 6**: In the clipboard, users can have multiple items stored. Seen in this example of the floating clipboard, there is one picture, two links, and one body of text that has been copied into the clipboard.*

#### History

Within the Dropbox web browser or application, users are able to access Dropbox Clip’s history. Similar to an internet search history, users are able to see all the items they’ve copied, not just the six that appear in their toolbar (Figure 7). The toolbar can only hold six items to reduce cognitive overload. The history function enables long-term retrieval of media if needed by users, even though the main use case for this feature would be short-term retrieval. 

![Clip History](../images/ClipHistory.jpg)
***Figure 7**: Users are able to view a full history of their copies within the Dropbox web browser. By selecting a piece of content from this view, users can copy and download the content.*

#### Download
On both mobile and desktop, users can directly download media to their local device. On desktop, this feature includes a long haptic press on images and videos in the clipboard, allowing them to save to their camera roll (Figure 8). On the desktop, from the toolbar menu users are able to click the “Download” icon, and the media can be found in their downloads folder. Other forms of media, such as texts and links, cannot be downloaded.

![Download](../images/download.png)
***Figure 8**: (left) On Clip’s desktop view, images and videos have download icons that users can click to save the media to their original device. (right) On Clip’s mobile view, users long-press on the content they would like to save and click “Save to Photos” to store that locally on their device.*

#### Privacy, Security, and Work Mode

There are three options that users have: Always, Work Mode, and Never. These options change the permissions that Dropbox Clip has for recording the clipboard history.

With Work Mode, users can specify when they want Dropbox to record a history of their copies (Figure 9). This may be used during work sessions when users know that they are going to use assets multiple times, but don’t necessarily want to search for them over and over again. The applications that might use this setting are apps like Figma, Adobe Products, or Google products. On a day to day basis, users might not want Clip to record a history of these applications due to confidential information or the sheer volume of copies made in these applications. However, when sitting down to work on a certain project, it could be useful to have copies from that session on hand. Work Mode allows for that choice.

| Security Option | Explanation | Example |
| --------------- | ----------- | ------- |
| Always Allow    | Enables Dropbox Clip to record copy history all the time | Microsoft Word, Notes |
| Work Mode       | Enables Dropbox Clip to record copy history only when Work Mode is enabled | Internet Browser |
| Never Allow     | Dropbox Clip is never able to record the copy history for this application | Password Managers |

These options can be found in the system preferences and permissions for specific applications. Similar to text messages, all copies are encrypted between the users and their own devices. Therefore, Dropbox does not have access to the files that are copied, just the encrypted version. These conditions will be a part of a Terms & Condition clause that users can accept or deny when first installing Dropbox Clip.

![System preferences for Dropbox Clip](../images/settings.png)

***Figure 9**: Within the permissions for Dropbox, there are settings that determine the privacy of users. This is found in the dropdown menu with the current state of “Always Allow” selected.*

## Next Steps

With only ten weeks for this project, we knew we would have to limit the scope of our research and designs. During our initial research phase of the project, we found many interesting insights that we weren’t able to explore due to the time and resource restraints for the project. We suggest that further research be conducted to explore the following topics:

- Gen-Z sharing files with other team members 
- Gen-Z’s relationship with their computer’s desktop as a temporary storage space 
- Organization of cloud vs. local storage 
- How Gen-Z uses screenshots

Within the Dropbox Clip application, there are also many features that we discussed, but knew would not be in the scope of our project:

- Creating a new keyboard command that accesses the floating clipboard
- A floating clipboard for tablets
- A “favorites” feature for frequently copied items
- Customizable amount of items in the clipboard

Although this project had its trials and tribulations, we hope to see Dropbox continue with this concept and research in the future. Gen-Z creative students is an extremely user group to look into, and with continued research in their behaviors with files and workflows Dropbox could create something very impactful for the users’ work. 