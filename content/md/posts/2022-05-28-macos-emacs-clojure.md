{:title "Clojure,  macOS, and Emacs bliss"
 :draft? true
 :layout :post}

After 10 years of using `vim`, in 2015 I decided to learn `emacs`, and
I've been at it ever since. Let me explain my `emacs` setup, and see
if I can convert any wayward developers to join the true way.

## The Basics

Firstly, my main driver is a Macbook Pro M1 14". These are fantastic
machines, and though they are expensive they are well worth it. I
prefer macOS for software like Zoom, Apple Mail, Messages, Spotify,
Cron, Front, etc. I use this laptop for business and for coding.

I also run a clandestine Linux deskop running Arch Linux with my own
custom build of [`dwm`](https://dwm.suckless.org/), but that's a story
for another day. Today we're covering macOS.

### The best version of `emacs` for macOS

There are several versions of `emacs` out there, but you should use
the [Mitsuharu
Yamamoto](https://bitbucket.org/mituharu/emacs-mac/src/master/) one
(available [here](https://github.com/railwaycat/homebrew-emacsmacport)
as a homebrew tap).

## Configuring `emacs`

Check out my [`.emacs.d`](https://github.com/amackera/emacs.d) for
inspiration on configuration. I keep my `emacs` packages in sync with
[Cask](https://github.com/cask/cask) and
[Pallet](https://github.com/rdallasgray/pallet).

## UI

## Helpful modes

### Org Mode

### CIDER

### mu4e

### circe

If you want IRC inside your emacs, by all means give
[circle](https://github.com/emacs-circe/circe) a try. In a past life I
have been a heavy IRC user, but these days I far prefer email
