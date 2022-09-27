# 💻 Setting Up Your Mac 💻

Hello and welcome! We are assuming that if you are on this page, you are looking for instructions on how to set your Mac up to be ready to start day one of our course!

The software outlined in this document is not an exhaustive list — just the basics to get you started on your first week at Makers.

> **DISCLAIMER:** NO WARRANTY OR SUPPORT. By continuing to follow the instructions within this document, you expressly acknowledge and agree that use of this or any Makers guides, and use of any Software and Services listed is at your sole risk and that the entire risk as to satisfactory quality, performance, accuracy and effort is with you.

## 🚦 Starting Point 🚦

So you have a new Mac! The rest of this guide expects that you have already got a functioning installation of a recent and supported version of Apple's OS X, that your machine's hardware is functioning correctly and you have admin privileges (or at least enough permissions to install software as a root user).

If you are new to macOs, you might not be aware that when you download an application file, you must drag it to the `Applications` folder. This is particularly important in the case of something like text editors, for writing code in.

You're also going to be installing a lot of things using the `terminal.` You'll feel like a real hacker! But there are two things it's important to bear in mind here:

* When using the terminal, there's a rule of thumb: "No news is good news". What this means, is when using the terminal, you mostly get feedback when something has gone wrong — success messages are nice, but not to be expected at the command line!
* When installing things in the terminal, a lot of text appears. It's important to pay attention to this because:
  * If something goes wrong, useful error messages will be there for you to copy and paste when looking for help
  * Further instructions might appear which are necessary to follow

## 🧰 XCode Command Line Tools 🧰

IMPORTANT: we only require the _command line tools_ part of XCode — not the full development suite (which is a considerably large download). You are welcome to install all of XCode if you have the time and bandwidth — but it's not necessary, nor will we mention it again in this guide.

There are a few ways to install XCode Command Line Tools:

**Route 1: `Run xcode-select --install`**

Copy and paste this into your terminal:

```bash
xcode-select --install
```

**Route 2: `Use a command to trigger the installation`**

Here are examples of commands that should trigger a prompt to install Xcode Command Line Tools when pasted into your terminal:

```bash
clang
```
`clang` is a compiler that turns C/C++/Objective-C source code into an executable program. You are unlikely to see this again on the course.

```bash
gcc
```
`gcc` is the GNU compiler. You are unlikely to see this again on the course.

**Route 3: `Go to developer.apple.com/downloads`**

If you fancy signing up for a free Apple Developer account, you can access a download for XCode Command Line Tools [here.](https://developer.apple.com/downloads/)

## 💎 Ruby Version Manager (RVM) 💎

Currently the main language we teach on the course is Ruby. Sometimes only certain versions of Ruby are compatible with certain projects (this is something you will experience a lot as a developer).

Your Mac should come with a version of Ruby pre-installed, but you will need a tool that lets you have multiple versions of Ruby available to you, and that makes it easy to switch between them easily. Enter your new friend: Ruby Version Manager (RVM).

At present there is only one route to install RVM that we would recommend: visit [rvm.io](https://rvm.io) and follow the installation instructions.

If you are in too much of a rush, you could just paste the following command into your terminal:

```bash
\curl -sSL https://get.rvm.io | bash -s stable
```

But we highly recommend learning a little bit about all of the software you're installing. Understanding how to use `rvm` to install and use different versions of Ruby is quite important on the course.

### Using RVM to install Ruby

Next, you're going to use RVM to install Ruby.
Use the following commands to install version 3.0.0 of Ruby and then set it as the default to use going forward.

```bash
rvm install 3.0.0
rvm --default use 3.0.0
```

Once you've done that, verify that you’re now using an RVM-managed version of Ruby by running the following command:

```bash
which ruby
```

If it prints something that looks like

```bash
/Users/<your username>/.rvm/rubies/ruby-3.0.0/bin/ruby
```

or

```bash
~/.rvm/rubies/ruby-3.0.0/bin/ruby
```

it means that the installation was successful.

**If you run into any problems at this point, ask your cohort for help and then reach out to a coach if you are still blocked.**

## ☕ Homebrew ☕

Homebrew is a package manager for macOS (and also works for Linux). If you're not sure what a package manager is, you can think of it as an easy way to install a bunch of software.

Within the development community, a lot of useful software can be installed using the command `brew install`.

But first, you need to install Homebrew. [You can find instructions on their website here,](https://brew.sh/) or you can paste the following in your terminal:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## 🎨 Visual Studio Code 🎨

You'll need an Integrated Development Environment (IDE) to write your code. We highly recommend VS Code, [which you can download from here,](https://code.visualstudio.com/download) or if you want to use `brew`, by running the following in your terminal:

```bash
brew install --cask visual-studio-code
```

Additionally, we **highly** recommend [following these instructions to enable you to launch VS Code from your terminal.](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line) 👍

## 🤖 Google Chrome 🤖

Love it or hate it, Google Chrome is a powerful modern web browser with excellent debugging tools. [You'll want to download a copy from here,](https://www.google.com/chrome/) or if you want to use `brew`, by running the following in your terminal:

```bash
brew install --cask google-chrome
```

## 💬 Slack 💬

We use Slack a lot to talk to each other. [You'll want to download it from here,](https://slack.com/intl/en-gb/downloads/mac) or if you want to use `brew`, by running the following in your terminal:

```bash
brew install --cask slack
```

## 🎥 Zoom 🎥

Currently our video conferencing software of choice is Zoom. We do a lot of remote work, and even some of our cohorts are fully-remote. So you'll want to install this if you intend to join the fun! [Download Zoom from here,](https://zoom.us/download), or if you want to use `brew`, by running the following in your terminal:

```bash
brew install --cask zoom
```

## 📺 iTerm 📺

While the native macOs Terminal application is perfectly good, we think that iTerm is better! [So why not grab a copy from here (any version will do),](https://iterm2.com/downloads.html) or if you want to use `brew`, by running the following in your terminal:

```bash
brew install --cask iterm2
```

## 🌈 Oh My ZSH! 🌈

For the slickest-looking terminal on the block, one requires a ton of time and patience — or you can just install [Oh My ZSH!](https://ohmyz.sh/) How? We've got you covered! Simply drop this in your terminal:

```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Besides being very pretty, this will actually be very useful to you when you start working with `git` on the course!

## 👾️ Now it's time to start `PROGRAMMING!`👾️
