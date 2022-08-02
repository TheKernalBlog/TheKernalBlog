---
published: true
---
Emacs can make your writing and coding more efficient, be used as a standardized framework for hundreds of Elisp applications, and be used as a desktop environment. But there's one thing that I've always wanted Emacs to do. I want Emacs to fix my life. I want this Elisp interpreter to make me a better, more productive, and more focused person. Well as it turns out, there is one application out there that does just that. Org Agenda has deccended from the heavens, like a graceful angel spreading joy and goodness, to fix your scheduling. So, if you too would like to be graced by this holy application, I will demonstrate the basics of how you can install, set up, and use Org Agenda on Emacs.

# Creating & Sourcing Agenda Files

It is most likely that you are going to want several different files for all of the different things you need to do in your day-to-day life. For example, I have four files called, 'School.org', 'Blog.org', 'Personal.org', and 'Other.org'. Most likely, you are going to want to put these in a directory of their own. One common place for these files is *~/org/agenda/*, but many people also keep them in *~/Documents*. However, it really doesn't matter where you put them, just make sure that they're somewhere.

And once you have these files created in their respective directory, you need to edit your init file. You just need to point Org Agenda to the correct files, by making use of the 'org-agenda-files' setting. Here is an example with two files, however there can be as many or as few as you desire.

    (setq org-agenda-files (list "~/DIR/FILE.org"
                             "~/DIR/FILE2.org")

# Using The Sourced Files

Now that you have the files set up, you have to get to creating TODO's, scheduling, and completing them. I always like to start off with a level 1 heading for the task that I would like to accomplish. Here is an example.

> * Write About Org Agenda

Then, I add a subheading for the type of task it is.

> ** Tutorial

And from there, I start creating TODO entries. You can either type 'TODO' before the task you would like to complete, or type "**C-c C-t**", which will bring up a menu where you can turn the current line into a TODO entry. You aren't just restricted to 'TODO' either. You can use 'DOING', 'DONE', and 'CANCEL', which are all just as valid.

> DONE Research and get basic outline

> TODO Finish Writing and upload

Unless you just want a simple list, you are going to need to schedule your tasks. This can be done with the keybinding, "**C-c C-s**". Once you enter the keybinding, Org-Calendar will pop up, and you have to pick what day and time you would like to schedule your task.

Once you put all of these aspects together, you are left with something that looks a little like this.

    * Write About Org Agenda
    ** Tutorial
    *** DONE Research And Get basic outline
    CLOSED: 2022-06-23 THu 00:43 SCHEDULED: 2022-06-22 Wed
    *** TODO Finish And Upload
    SCHEDULED: 2022-06-23 Thu

# Using The Agenda

Org agenda can be launched with "**C-c a**". And from there, you have a few options. There are a total of 14, but the most important are as follows.

### Agenda View
> Displays the agenda for the current day or week.

Can be launched with "**a**"

### TODO View
> Lists all TODO entries, from any time period.

Can be launched with "**t**"

### Search
> Prompts You To Search Through All TODO Entries

Can be launched with "**s**"

And once you have the Agenda open, you can mark your tasks as completed using the "**t**" keybinding, which will open up the same menu as before, where you can mark it as 'DONE', 'CANCEL', or even 'DOING'.

# You Did It!

You can now properly create, schedule, search, and complete items on a virtual agenda from within Emacs. This will allow you to have a propper, reliable, and freedom-respecting Agenda, without having to download a super heavy calendar app, or worry about keeping a pen & paper with you. And while this may not be the most robust Org Agenda tutorial in the world, it should be enough to use it effectively, with some room to grow and learn about this amazing program.
