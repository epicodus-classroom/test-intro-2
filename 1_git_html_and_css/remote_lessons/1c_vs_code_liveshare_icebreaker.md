In this lesson, we'll cover setting up a VS Code Live Share session. You'll take part in an icebreaker with your pair, learn good pairing etiquette, and get an opportunity to practice hosting a VS Code Live Share session.

This ice breaker is a group exercise. If you haven't found a pair to work with from your dev team, find one now. If there is an odd number of people in your dev team, there will be one group of three. If you are a remote student and you have not set up a direct message with your dev team or your pair, please do so now. As necessary, revisit this lesson on [Direct Messages in Discord](https://www.learnhowtoprogram.com/introduction-to-programming/getting-started-with-working-remotely/direct-messages-in-discord) for review.

**Both in-person and online students will practice using VS Code Live Share with this icebreaker.** 

Students who are working in person will find another pair to do the icebreaker with. This means that one pair on one computer and work with another pair on another computer. There will be at least 4 students in the icebreaker group, if not more due to groups of three. If possible, work with your neighbor or a pair close by so you can talk about any issues that come up. If there's an odd number of pairs in the class, make a group of three pairs, or join another group of two pairs to make two groups of three or more.

Students who are working online will do the icebreaker with their pair (or group of three) for the class. 

**Goal:** We have several goals in this lesson:

* Practice using VS Code Live Share.
* Learn pairing communication techniques.
* Get to know your classmates better!
* Communicate with your dev team and help out others as needed.

**Note:** If you have technical difficulties during this exercise and you aren't able to cover the icebreaker questions in much depth (or at all) that is completely fine. Some students will spend the entire time debugging VS Code Live Share. While that _is_ frustrating, getting you and your pair up and running on VS Code Live Share is the #1 goal of this lesson.

## Set Up VS Code Live Share

---

Once you are in your icebreaker group, you're ready to start using VS Code Live Share. For online students, choose one person to host the first session. For in-person students, choose one pair to host the first session. Don't worry — everyone will get a chance to practice hosting a session so it doesn't matter who goes first. 

Online students should also have a Discord voice channel (or a video call if preferred) with your pair. This is not a silent exercise and you'll generally be using Discord to communicate while you use VS Code Live Share to write code together.

Next, **everyone should do the following steps regardless of whether you are hosting** — don't forget, even if you're not hosting yet, you will be in just a few minutes. For in-person students, you only need to follow these steps once on each computer.

* Navigate to your desktop from the terminal (using commands you learned in [Interacting with the Command Line](https://www.learnhowtoprogram.com/introduction-to-programming/getting-started-with-intro-to-programming/interacting-with-the-command-line)). If you are on a Mac or PC, the command will likely be `$ cd ~/Desktop`.

* Create a directory on your desktop called `icebreaker` by typing `$ mkdir icebreaker` in the terminal.

* Navigate inside the `icebreaker` directory (`$ cd icebreaker`) and create a file called `hi.txt`. This is just a text file — we are keeping things very simple here because we're focused on practicing VS Code Live Share, not worrying about code yet. A quick reminder: you can create the file with the following command: `$ touch hi.txt`.

* Type `$ code .` in the terminal (from inside the `icebreaker` directory) to open VS Code. Remember, you need to run `code .` in the directory of the project you are working on — not a directory higher up in the file tree. You will be sharing access (including write access) of all these files with your pair. For instance, if you were to run `code .` in the root directory of your computer, you'd be giving your pair both read and write access to _every_ file on your computer — not just the files in your project. This is a security risk!

* Make sure that `hi.txt` is showing in the left-hand pane of VS Code. If the file tree isn't showing, click the top left _Explorer_ icon that shows two overlapping squares to show the file tree. See the image below.

<img src="https://learnhowtoprogram.s3.us-west-2.amazonaws.com/INTRO/week1-html-css/remote_images_2021/screenshare-file-tree.png" alt="File tree is showing — and the icon for the Explorer is circled." style="width:50%" />

In the image, the file tree is showing (we can see `hi.txt`). The _Explorer_ icon in the upper left corner is also circled. You can click on this icon any time to toggle the file tree. If the file still isn't showing, you're probably not in the right directory or the file wasn't properly created. Make sure you are in the `icebreaker` directory, type `$ ls` to see a list of files in the directory (which should show `hi.txt`) and then type in `$ code .`.

* Once you've ensured that the project you want to share is open in VS Code, you're ready to use Live Share! Click the circle with an arrow on the left side of your screen to access Live Share. That is the bottom icon on the left in the image below. (This icon will be added after you've installed Live Share.) The user interface (UI) of programs change often, so if your icon looks slightly different, or doesn't have the same highlight, that is normal.
 
![Image of tab with circle with arrow on left side and Live Share menu options.](https://learnhowtoprogram.s3.us-west-2.amazonaws.com/live-share-images/start_liveshare_session.png)
 
* Make sure the file you're working on is saved. Live Share won't work on new, unsaved files. 

* Then, start your collaboration session. Only the current icebreaker host should start their session. There will be one session hosted by one person/computer that everyone else will join. (Later on, we will switch who is hosting). Since the UI of Live Share changes periodically, you may have one of two options to start your Live Share session: a link that says _Start collaboration session_, or a button that says _Share_. In the image above, you can see a button that says _Share_. If any of the words are cut off in the Live Share pane, use your mouse to widen the left-side pane in VS Code.

*  When you start a Live Share session, a link will automatically be copied to your clipboard that you can share with your pair. Once you get that link, share it with your pair via your Discord direct message (DM). Students who are studying in-person should also share their links via DM.

### A Few Notes

If this is your first time starting a Live Share session on your personal computer, you may be prompted to give the program permissions. Select the option that you are comfortable with. You may also be prompted to sign in via your GitHub account, like in the image below. We suggest that you sign in to your Live Share sessions, so that you are listed by your user name and not "anonymous". Typically you will sign in once, and VS Code will save that information for future sessions.

![This is a prompt that is asking you to sign into your GitHub account.](https://learnhowtoprogram.s3.us-west-2.amazonaws.com/live-share-images/sign_in_to_join_liveshare_session.png)

As we noted above, when you start a Live Share session, a link will automatically be copied to your clipboard. If you need to get the link again, just click on _Invite participants_, which is highlighted in the image below.
 
![ Click on the "Invite participants link" on left side of screen.](https://learnhowtoprogram.s3.us-west-2.amazonaws.com/live-share-images/image2.png)

## Joining a Live Share Session

---

### [Joining a Live Share Session](#joining-a-live-share-session)

There are a couple of ways to join a Live Share session. We'll start by sharing one method, discussing a few options, and then cover another method. We suggest that you read through this whole section before attempting to join a Live Share session for the first time.

Everyone who is not hosting should join the Live Share session using the URL that your pair has given you.

#### Method #1 — Joining a Live Share by Following the URL

The Live Share URL that your pair shares with you is also a link that you can click to join the session. This is the easiest way to join a Live Share. However, you will have to do some configuration when you are joining a Live Share for the first time.

After you work through the configuration options (below), you will be able to see and work in any file in the `icebreaker` project.

#### Option to Join Live Share Session in Browser or in VS Code

If this is the first time you are joining a Live Share session, you will encounter a dialogue box that will ask you if you want to _Continue in Web_ or _Open in Visual Studio Code_. See the image below as an example of this dialogue box. 

![Dialogue box asking you to select whether to open links in browser or via the web.](https://learnhowtoprogram.s3.us-west-2.amazonaws.com/live-share-images/option_to_use_live_share_in_browser_or_on_computer.png)

We strongly suggest that you select to open the project in VS Code. Why? The VS Code installed to your computer has access to your computer's terminal, and it also has all of your configurations and extensions enabled. When you use VS Code in the web browser, it will not have these configurations set up, nor will it have access to your computer's terminal. 

It's important to know that whatever option you first select (continuing in web or in VS Code), this preference will be saved. You can change this option later via your VS Code settings. Let's look at that next. 

#### Changing Your Live Share Launch Settings

If you decide you want to use Live Share in the browser, or otherwise, here's how you can access the launch settings for Live Share in VS Code.

1. Open VS Code settings.
2. Make sure you are editing `user` settings. This is in contrast to `workspace` settings. User settings are globally applied to all VS Code sessions, whereas workspace settings are only applied to the VS Code window you are currently in.
3. Search for `Live Share: Launcher Client`.
4. Set the value for the launcher client to `visualStudioCode` to launch Live Share sessions in your local VS Code. Select `web` to launch Live Share sessions in the browser. Note that `visualStudio` is a separate program that we will not work with in this program.

#### Option to Sign into Your GitHub Account

If this is your first time joining a Live Share session, you may be prompted to _Sign in_ or _Continue as anonymous_, like in the image below. When you sign in, you will do so via GitHub. We suggest that you always sign in to your Live Share sessions, so that you are listed by your user name and not "anonymous". Typically you will sign in once, and VS Code will save that information for future sessions.

![VS Code Live Share will prompt you to sign into your GitHub account.](https://learnhowtoprogram.s3.us-west-2.amazonaws.com/live-share-images/sign_in_to_join_liveshare_session.png).

#### Method #2 — Joining a Live Share Session in VS Code

Here's another way to join a Live Share session. Though it's not as convenient as clicking on a link, it's helpful to know another option, and you may find this method preferable! Follow these steps:

*  Open VS Code (if it isn't open already), or open a new VS Code window by selecting _File_ > _New Window_.
*  Open the Live Share pane by clicking the Live Share icon from the navigation bar. 
*  Select the option to join a collaboration session: either a button that says _Join_ or a link that says _Join collaboration session_.
*  VS Code will open an input at the top of the screen, as highlighted by the orange box in the image below.
*  Enter the URL of the collaboration session (the URL that your pair has shared with you) into the VS Code input and hit enter.

You will now be able to see and work in any file in the `icebreaker` project!

![Enter the collaboration session URL into the input after you click "join" or "join collaboration session"](https://learnhowtoprogram.s3.us-west-2.amazonaws.com/live-share-images/join_liveshare_session.png)

## Icebreaker — and Good Pairing Etiquette

---

Now that you've started a VS Code Live Share session, it's time for an icebreaker. Everyone will get a chance to answer a few questions via VS Code Live Share.

Before we do that, though, let's cover some basic remote pairing etiquette. You both have the ability to type and edit VS Code files in the project right now. It's kind of like being in a car together and you both have steering wheels. Obviously, it wouldn't be good if you both tried to steer at the same time!

One person should answer one question at a time. When they are finished, let your pair know.

First, the host will copy the following questions into `icebreaker.txt` and _save_ the file.

**Note:** There are five questions below. You are not required to answer them all! We've provided additional questions so you can choose not to answer a few of them if you'd prefer not to. This is supposed to be a fun exercise, not to put anyone on the spot.

```
What is your favorite time of the day and why?

What is your dream job?

What are three of your favorite foods?

What would be the most exciting scientific discovery ever? (Examples: time travel, recreating dinosaurs, flying cars, etc.)

Would you rather travel back in time to meet your ancestors or to the future to meet your descendants? Why?

What is your most used emoji?

What’s your favorite sandwich and why?
```

Next, you and your pair will alternate answering each question by _typing your answer_ in VS Code and then saving the file. In-person students will be working in groups of 4 or more, so in this case, each person should answer one question, save, and then move to the next person in the group.  _Be sure to answer one question at a time and then alternate._ This is similar to how we conduct pair programming when we are actually coding — the difference is we generally expect pairs to switch driving (typing and controlling the keyboard) every 20 minutes or so when coding.

You may want to review the pointers in [Remote Pairing Etiquette](https://www.learnhowtoprogram.com/introduction-to-programming/getting-started-with-working-remotely/remote-pairing-etiquette). Here are a few key points to follow in this icebreaker exercise.

**When you are driving (typing):**

* Vocalize what you are thinking and doing. So as you answer the question in VS Code, vocalize your process as well.

* Be proactive about turn-taking. When you are done answering a question, communicate clearly that you are ready for your pair to drive.

* Make sure to actively switch after you answer a question!

**When you are not driving (observing):**

* Don't take over the keyboard without checking in first.

* Don't give someone a hard time about the speed of their typing or typos. Once you are coding, you will want to point out typos in the code — but remember, you should always endeavor to do so in a constructive manner.

* Listen with the intent of listening, not responding. This means focusing on active listening skills. These skills will be essential for you in your next job — even more so than your coding skills.

## Alternate Hosting

---

Once you are done, it's time for the next person to do the same thing! End the remote sharing session, so the next person can host. Follow the same steps to host a session listed earlier in this lesson. Move onto the next lesson once everyone in your group has hosted once.

This time, you'll answer the following questions. Once again, you don't need to answer every single question — we've added a few extra if there are a few you'd prefer not to answer.

```
What was the best piece of advice you ever received? (Or a generally good piece of advice...)

What was the worst and/or best job you ever had?

Would you rather be able to fly or teleport? Why?

What is your favorite place in the world?

What is your favorite TV show, movie, or book?

If you could go to Mars, would you? Why or why not?
```

We've included more questions below for a group of three. Remember, each person (whether that's two, four, or more people) should get a chance to host a live-sharing session on VS Code. If you are pair programming (only two people), you can skip the questions below.

```
What is your favorite animal or plant? Why?

What is your favorite color?

What is your favorite band or your favorite type of music or your favorite lyric?

If you were a character in a movie, television show, or book, which would you be?

Would you rather take a sight-seeing trip in a hot air balloon or a submarine? Why?

What's your favorite decade and why?

You can visit any fictional time or place. Which would you pick?
```

By this point, you and your pair should have both successfully hosted a VS Code Live Share session. If you have any technical difficulties, first reach out to members your dev team and then reach out to your instructors.

We're almost ready to start coding! In the next lesson, you'll start learning about Git and the terminal. If you are an online student, you will also practice sharing your screen.
