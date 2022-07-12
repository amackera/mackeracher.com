{:title "Clojure,  macOS, and Emacs bliss"
 :draft? true
 :layout :post}

After 10 years of using `vim`, in 2015 I decided to learn Emacs.
I've been at it ever since. Let me explain my Emacs setup, and let's
see if I can convert any wayward developers to join the way of the `()`.

## The Basics

Firstly, my main driver is a Macbook Pro M1 14". These are fantastic
machines, and though they are expensive they are well worth it. I
prefer macOS for software like Zoom, Apple Mail, Messages, Spotify,
Cron, Front, etc. I use this laptop for business and for coding. This
basis provides a stable platform to work from every day, with only
minor disruptions to update system packages and applications.

I also run a clandestine Linux deskop running Arch Linux with my own
custom build of [`dwm`](https://dwm.suckless.org/) under the table,
but that's a story for another day.

### The best version of Emacs for macOS

Unfortunately, by using macOS, we've robbed ourselves of *some* of the
magic that ships to GNU/Linux users with the venerable [GNU
Emacs](https://www.gnu.org/software/emacs/) project. To recapture the
performance and system-level integrations provided out-of-the-box to
Linux users, we will need to use a special macOS build of Emacs.

There are several versions of Emacs out there, but you should use the
[Mitsuharu
Yamamoto](https://bitbucket.org/mituharu/emacs-mac/src/master/) one
(available [here](https://github.com/railwaycat/homebrew-emacsmacport)
as a homebrew tap). This one provides good macOS GUI support,
pixel-based mouse wheel smooth scroll, keyboard shortcuts, clipboard
support, HiDPI support for high resolution monitors, and more. It's
legit.

Install it via [Homebrew](https://brew.sh/):

```bash
brew tap railwaycat/emacsmacport
brew install emacs-mac
```

## Configuring Emacs

Check out my [`.emacs.d`](https://github.com/amackera/emacs.d) for
inspiration on configuration. I keep my Emacs packages in sync with
[Cask](https://github.com/cask/cask) and
[Pallet](https://github.com/rdallasgray/pallet).

## UI

I rock the
[`kaolin-galaxy`](https://github.com/ogdenwebb/emacs-kaolin-themes)
theme. There's no reason to ever code on a light background, so it's
dark mode only for me. It looks like this:

![Emacs Screenshot](/img/Emacs-Anson.png)

Notice how much it looks like this website. It's not an accident, I'm
actually that uncreative.

## Helpful modes

### Org Mode

A no brainer if you already use Emacs. [Org
Mode](https://orgmode.org/) is a popular Emacs major mode for keeping notes, writing docs, computational notebooks, planning projects, tracking tasks, tracking time, and more! Org Mode alone is enough of a reason to switch to Emacs.

Org Mode is like having a Jupyter Notebook for everything you write.

### CIDER

This one's specifically for the Clojure fans out there. CIDER is a useful major mode for Emacs that provides interactive programming via a running Clojure progress. You can compile, debug, look up docs, run tests, and more, all from within Emacs via CIDER.

### mu4e

It's possible to consume and create email from within Emacs. After all, email is only text, and if it's text Emacs can edit it. I've tried a few packages and [`mu4e`](https://www.djcbsoftware.nl/code/mu/mu4e.html) seems like the best. I couldn't stick with it, but maybe you can.

### circe

If you want IRC inside your Emacs, by all means give
[circle](https://github.com/emacs-circe/circe) a try. In a past life I
have been a heavy IRC user, but these days I far prefer email
