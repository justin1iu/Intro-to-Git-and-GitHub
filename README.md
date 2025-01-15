# Intro to Git and GitHub

This lesson introduces key concepts that we will use throughout the course.

Before any of that, though, I'll need you each to sign up for a GitHub
account if you don't already have one: https://github.com.

(Before the complaints start rolling in: I know, I'm sorry to make you use a Microsoft-owned
product. But they provide a generous free tier for computing and allow you to set up and work in a
cloud environment without needing to maintain an environment on your own machine.)

## `git` versus GitHub: What's the difference?

`git` is a command line utility for version control.

GitHub (or GitLab, or Codeberg, etc.) is a company that provides remote
hosting for git **repositories**.

> Discuss: Read the above definitions again. What questions do you have?

## Forking, committing, pushing, and pulling

You'll hear these words a lot when we talk about moving code around with `git`.

### Forking

**Forking** means creating a version of a repository that you own. Try it now
by forking this repository from the TuftsIntroDH organization to your personal
organization on GitHub.


### Committing

**Committing** refers to the process of adding, removing, or changing the files in a repository.
A **commit** is a snapshot of a moment in time at the repository. You can think of it like track
changes with super powers.


### Pushing

**Pushing** means sending your **local** changes to a **remote** host. In this course, you probably
won't do much pushing directly, as you'll be working in codespaces. Rather, you'll open **pull
requests**, which are a way of asking another version of the repository to accept your changes.


### Pulling

**Pulling** means adopting changes that someone else made to a repository that you don't yet have
locally. You might need to do this if we need to update a repository after you've started working
on.

In the ideal scenario, you'll be able just to commit your local changes and then pull in the remote
changes. However, if `git` determines that two changes apply to the same location, it will create a
**merge conflict**, letting you know that it couldn't automatically merge the changes from the two
versions of the repository.

The key to merge conflicts is to remain calm. Just search for `>>>>>>` in the files that have
changed, take a look at the commits associated with each version, and decide which one to keep --
or, somewhat less commonly, how to reconcile the two versions manually.

## Codespaces

GitHub provides a service called **Codespaces**: these are on-demand virtual machines that
start with all of the code in a repository. They run an online version of [Visual Studio
Code](https://code.visualstudio.com), a free and open-source **text editor** from Microsoft.

Open a codespace in your fork of this repository.

> Discuss: What do you see? What stands out in the codespace environment? What's confusing?

## Creating new content

1. Create a file called {YOUR_NAME}.md in your codespace.
2. Add your name to the top of the file so that it looks like this:

```markdown
# Your Name
```

3. Go to the "Source Control" tab in your codespace. What do you see there?
4. Go ahead and **stage** that file, and then **commit** the result with an informative message.
5. Finally, open a **pull request** to ask for your changes to be merged into the **upstream** (= main) version of this repository.


## What happens during a pull request?

Let's take a close look at some of these pull requests together.

> Discuss: What do you notice when opening a pull request? What does GitHub make it easy to say, and what's more difficult to notice?


## Merging and pulling

I'll just need a second to merge all of your changes into the main repository.

...

Okay, with that out of the way, now each of your local repos looks quite different from the main repo.

> Discuss: How can we get them in sync?

## Further changes

In the same file that you have created -- i.e., the file with your name on it and in it -- add a
few biographical details. You might start with your year, your major/minor, extracurriculars, fun
facts, etc.

Use this as an opportunity to experiment with [GitHub-Flavored
Markdown](https://github.github.com/gfm/). Add some links to resources you find handy, add some
images or gifs (keep it PG, please), and generally try to see if you can figure out a bit of how
Markdown works.

## Wrap-up

Now commit those changes and open new pull requests. If everything goes smoothly, we'll now have a
repository where we can get to know each other. 🥳

> Discuss: What parts of this workflow did you find challenging? What are some things you might need
to watch out for when working with `git` and GitHub?

> Discuss: Can you remember the difference between `git` and GitHub?
