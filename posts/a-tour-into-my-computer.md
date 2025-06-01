:warning: Disclaimer :warning:

*This article is a great snapshot of what my Linux experience was like at the
time of writing it (2022). Obviously, as time goes on, my habits change. Please
keep that in mind while reading!*

-- Tina from 2025.

Like many, I spend a lot of time on my computer. I want the time I spend on my
computer to be pleasant, but since I also work on my computer it has to provide
me with an easy-to-use and productive environment.

As of right now, I mainly use 2 different computers, I work on both but I play
video games on only one of them. One is a desktop computer, the other is a
laptop.

For most of my everyday tasks, such as browsing the web, watching anime,
listening to music, doing school activities, working on personal projects, and working
for companies, I use Linux. For playing games I use Windows. As such I do not
have Windows on my laptop.

I'm not forced to use Linux, either by my current job or school. I use Linux
purely by choice because I find it way more satisfying to use. Obviously, as a
developer, I am also advantaged by the fact that I have access to way more
tools on Linux and they help with programming but also with regular usage, and
someone who does not have experience with IT may not find these tools
approachable.

![Clean desktop screenshot](https://tina.moe/assets/cloud/blog/computer-tour-2022/gnome-overview.png)
*What my desktop looks like on a new workspace*

![Linux desktop with several apps open](https://tina.moe/assets/cloud/blog/computer-tour-2022/linux-desktop-with-anime-and-twitter.png)
*Me very legally watching cultured anime with Twitter open on the side and a
Discord notification showing up*



[TOC]

## The distribution

There's a big misconception about Linux that what differentiates distros is the
"look" or "desktop". It is completely false and Linux desktop environments are
projects run by entirely different people than those who maintain
distributions.  However, what is true is that most distros offer a "standard"
variant for regular desktop usage, and those will come with a pre-installed
desktop on it.  This is often what is used as the basis for comparing
distributions by newcomers. But in fact, on Linux, the "desktop" you are seeing
is just one or multiple softwares being run, and you can swap them with
different ones just like you can pick between the different available Internet
browsers or media players.

So what makes distributions different from each other and what motivated my
choices? To me, the major points are as follow:

- The reason the project exists
- The way it is maintained
- The softwares "supported" and "pushed forward" by the project
- The "supported" ways to install more softwares

Now what I mean about "the reason it exists" is that some distributions exist
to provide a free and simple-to-use OS, while others may want to provide a
minimalistic base OS where people are supposed to have extensive knowledge
about the desktop ecosystem to gradually add components. Some are more about
technical differences like using a different init system, not using the GNU
libc or coreutils. Some are built around being tailored for a specific desktop
or software.

The other points are a bit easier to understand but it boils down to how
frequent the updates are, how decisions are made, can anyone contribute, are
some softwares better supported or integrated than others, what are the tools
available to install and manage softwares.

There are also some things that make it so I prefer using Linux over other
desktop OS and are true for every distribution. Linux makes it very easy to
package and distribute softwares so no matter the distro, you'll have a
centralized way to install, update and uninstall softwares, like the "store"
app you'd use on a smartphone. Another thing is the way everything about the OS
is broken into small components, making it so I can always replace parts of the
OS with alternatives, if I'm either dissatisfied with the way something works or
if I want to try a new hip cool thing.

With all that considered, my heart is with [**Fedora Linux**][fedora] for a
variety of reasons. They strongly advocate for free/libre software, something I
can resonate with because I'm a partisan of the open-source philosophy. They
provide updates very fast and very frequently, so you always have access to the
latest softwares and tools, sometimes even before the "cutting edge"
distributions. They not only provide updates very fast but they also support
the new additions to the Linux ecosystem way before everyone else.

Their strong stance on free software used to make it so you have to take a few
extra steps if you want non-free stuff, such as installing Chrome, Steam,
proprietary media codecs or graphics card drivers. However, they now provide
additional repositories for those popular non-free softwares which makes it
very straightforward to install them from the GUI.

![extra fedora repos shown in gnome
software](https://tina.moe/assets/cloud/blog/computer-tour-2022/extra-fedora-repos.png)

If you use the GNOME Software app, which does not require you to use GNOME, you
can easily extend it to not only show a restricted list of Fedora endorsed
applications but the entirety of what's available in both official and 3rd
party repositories, as well as from [Flathub](https://flathub.org). This way you
can basically use it to install almost anything that exists on Linux and very
easily. It can also handle updating your installed softwares, either manually
or automatically.

![searching "code" on gnome
software](https://tina.moe/assets/cloud/blog/computer-tour-2022/gnome-software-search.png)

New software releases are made available to the repositories almost as soon as
they drop, meaning you usually have updates available for at least something
daily. So you are always using the latest softwares available, which is good
for performance, hardware support, security, and programming.

Behavior-changing updates, such as major updates to the desktop environments or
to the underlying core components of the OS, are held back until the next Fedora
release, which happens every 6 months. Just like every other distribution, if
you are unhappy with this and want the latest versions immediately, you can use
the rolling release repositories instead of the fixed release ones.

I could brag for longer about why I love Fedora and think it's the perfect
distribution for almost every use case, but I need to talk about other stuff
too, otherwise, this will not be a computer tour but just distro wagging.

Before that, I'd like to mention that I've been using [Rocky Linux][rocky] on my
laptop instead of Fedora. This is my preferred distribution for servers. It is a
community copy of Red Hat Enterprise Linux, which is based on Fedora but with a
way slower release cycle and with an emphasis on stability and security. Using
it on my computer helped me understand a lot about it and thus made me more
capable with the way I manage my servers, however, it is always preferable to
have frequent updates for desktop usage so I might switch it back to Fedora
relatively soon.


[fedora]: https://getfedora.org/
[rocky]: https://rockylinux.org/

## The desktop

Even though I love talking about it, going on about distributions is probably
not the most interesting and exciting thing. So let's talk a bit more about the
desktop itself instead.

For approximately 4 years, I've been using either i3 or sway, which are
considered to be only window managers as opposed to desktop environments, due
to only being the software that manages windows, and requiring you to install
and configure additional softwares if you want other features you'd expect from
a desktop, such as a status bar, an applications launcher, notification popups,
things like that.

![my i3 setup in 2019](https://tina.moe/assets/cloud/blog/computer-tour-2022/old-setup-rofi-nemo-htop.png)
*My i3 setup back in 2019*

At that time, there were two things that charmed me with them. First the fact
that they are WMs meant it did not come with extra functionalities I don't need,
something I cared about because I was actively seeking unbloated solutions. The
other is that they provide a tiling windows workflow, meaning windows
automatically position and resize themselves to split your desktop into virtual
tiles when you open them, a workflow that I greatly appreciate because it
maximizes screen space usage, and if not done automatically I position the
windows in a similar way myself anyway, so having this behavior being the
default makes it less infuriating to use my desktop.

But in 2021 I eventually grew tired of it, mostly because I was unhappy with the
look it gave to my desktop to have to use different softwares for many core
desktop functionalities. Since they were all different projects, they all looked
different and so a lot of stuff looked out of place. While some apps like my
file explorer looked modern, the apps I used to manage my monitors or Bluetooth
connections looked way more dated. My notifications, launcher, and status bar all
looked very barebone and minimalistic. I started to really dislike this sense of
disunity, which is something I also dislike about Windows for instance.

This is why I started exploring more fully-fledged solutions, and after trying
multiple of them, the one that did the job the best for me was GNOME.

![gnome screenshot from wikipedia](https://tina.moe/assets/cloud/blog/computer-tour-2022/gnome-default-look.png)
*The default GNOME desktop as of version 41, from Wikipedia*

Just like with code editors and distros, there is a sort of war ongoing between
the users of each desktop, and GNOME has a reputation of being slow and
bloated. This was not my experience, however, and believe me I tried every major
desktop available on the market. I really liked the harmony between the core
apps and the themes and extensions ecosystem which makes it possible to tweak it
a lot and easily.

The "settings" app behaves like what you would expect from the one on Windows,
from it you can manage everything from your monitors, wifi connections,
printers, keyboard layouts, and obviously desktop customizations. This thus
replaced the many different softwares I was using on my i3 setup.

Using extensions, it was possible to recreate some of the tiling window manager
experience, and some bigger ones even had a very new and interesting take on it,
such as [PaperWM][paperwm] and [Material Shell][material-shell]. However, I
eventually backed down from using those bigger extensions as they had frequent
bugs and broke on major GNOME updates. But I am still able to recreate the i3
feel.

![two windows in a split view on GNOME](https://tina.moe/assets/cloud/blog/computer-tour-2022/gnome-split-view.png)

I use a theme called [Materia][materia] which is unsurprisingly based on the
Material Design trend and an icons theme called [Vimix][vimix-icons], which
play very nicely together.

I do not use much behavior-changing extensions, most of what I have installed
change the look, such as hiding certain elements, adding the distro logo on my
wallpaper or adding blur in several places.

Using [Tiling Assistant][tiling-assistant] I get a Windows-like prompt each time
I tile a window to an edge, asking me if I want to tile another open window to
the remaining space. It also enables me to create the "gaps" between windows,
which I love for how slick they look, and got used to them from when I was using
i3-gaps.

![current list of extensions](https://tina.moe/assets/cloud/blog/computer-tour-2022/gnome-current-extensions.png)

There are also some obscure configuration options I have tweaked, custom
shortcuts I added, some supporting scripts that I wrote, but those often change
over time and I'd have trouble remembering all of them but they made using
GNOME very pleasant to me.


[paperwm]: https://github.com/paperwm/PaperWM
[material-shell]: https://material-shell.com/
[materia]: https://github.com/nana-4/materia-theme
[vimix-icons]: https://github.com/vinceliuice/vimix-icon-theme
[tiling-assistant]: https://github.com/Leleat/Tiling-Assistant

## Keyboard focused workflow

We are used to the good old Alt+TAB to cycle between the different running
applications, and this behavior is available on practically every desktop. But
another habit I built over my years of using i3, is to use the Windows key + one
of the top row numbers to select specific applications. Using this instead of
alt-tabbing is way faster especially when you have many open applications. Think
of it like using the mouse wheel vs using the top row when playing CS:GO.

i3 did not really have this but instead, I made a habit of putting specific apps
on specific workspaces and using the Windows key + the number corresponding to
the workspace switched me to it. So Windows+1 would bring me to my "work", 2 to
my browser, and 3 to my chat apps. Thankfully, this is something that you can
easily reproduce on both GNOME and Windows by pinning some applications to the
status bar. When using Windows + a number, it will switch to the corresponding
application in your bar, or open it if there are no currently open windows of
it.  If the application is in another workspace, you will be moved to it. So I
just had to pin the terminal, Firefox, and Discord to my dock in this specific
order to get the exact same behavior and not trouble my muscle memory!

![workspaces overview screenshot](https://tina.moe/assets/cloud/blog/computer-tour-2022/gnome-overview.png)
*My pinned applications can be seen at the bottom of the screenshot*

One other very cool keyboard shortcut habit I picked up was from when I tried
Material Shell, where apps were disposed in an infinite 2-dimensional grid, and
you'd use Windows+W/A/S/D to move to the adjacent app in the grid. I imitated
this behavior by binding Windows+A and D to move to the workspace on the left
or on the right, which makes a lot of sense with the way the workspaces are
arranged visually, and is way easier to type than Windows+PageDown and PageUp,
the default bindings to navigate workspaces. Since I organize my apps into
workspaces a lot, having an easy to execute shortcut to navigate them is very
much appreciated.

## Consuming media

As you probably know, I consume a lot of Japanese media, namely anime, music,
drawings, and games. Now, for drawings, I mostly just browse Pixiv and Twitter
(or use [a bot I made to aggregate both in a Discord channel][art-companion]),
and for games, I just run them on Windows or use Valve's compatibility tool
"Proton" to run them on Linux. But about anime and music?

You may have noticed from the first screenshot, but I do not watch anime very
legally, not because I'm broke or because the services are not available in my
country, but mainly because I'm upset about the fragmentation of the services and
catalog. I do not want to have to subscribe to 10 different services to watch
the anime series I want to watch.

Piracy is nothing to brag about and I tend to make a point of avoiding talking
about it publicly as to not encourage it and let people decide for themselves if
they want to pirate content or not. But I'm not going to hide it if I'm
explaining the tools I use to watch content.

Usually, when I want to watch an anime, I hop on Nyaa Torrents, the mainstream
public tracker for Japanese culture content, and search for a HEVC/H.265
encoding of the episode I want to watch. Picking x265 encodes is way more
convenient because they weigh way less, it's usually between 300 or 400MB for a
24 minutes long 1080p episode, versus 1.2 - 1.6GB for the same episode in a more
traditional encoding.

Then I use [WebTorrent-CLI][webtorrent-cli] to download the file in sequential
order and link the output to my media player, which allows me to play and seek
through the file as it is being downloaded. This makes it no different from what
happens when you watch a video from a streaming service, except I'm exploiting
my bandwidth more efficiently thanks to the nature of torrenting.

For my media player I use [mpv][mpv], the most powerful and efficient media
player there is. I don't know how but they managed to outperform every other
existing competitor. This is somehow a recurrent theme with open source projects
with weebs in the list of main contributors.

When combined with the amazing tool [youtube-dl][youtube-dl], which allows
fetching media contents from YouTube but also a plethora of other platforms, mpv
will natively leverage it if you try to open an URL with it. Making it a very
convenient tool to have to play video or audio content from YouTube, Twitch or
Twitter when you do not wish to visit the actual website or the official player
is having trouble playing or not picking the highest available quality.

Finally, as far as music goes, I have a collection of albums that I have either
bought digitally or physically or downloaded from quality pirate sources, such
as bemaniso or DoujinStyle. I store this collection on a server I run in my
home, which is directly plugged into fiber Internet, and allows me to stream it
from anywhere in the world. I use [Jellyfin][jellyfin] as my media server and
UI when on PC, or the free/libre Android application [Gelli][gelli], a fork of
Phonograph that integrates with Jellyfin.

![screenshot of my jellyfin setup](https://tina.moe/assets/cloud/blog/computer-tour-2022/jellyfin-music.png)
*My Jellyfin music library and the player view*

If I'm downloading new music from a torrent, I effortlessly do so from a PC or
phone directly to my server using the modern torrent clients web UI
[Flood][flood], and make it download directly to my music folder, which will
update my library automatically.

![a screenshot of my Flood setup](https://tina.moe/assets/cloud/blog/computer-tour-2022/flood.png)

I usually go for V0 encodes as I'm not an audiophile enough to care about
lossless quality and they provide the best size/quality ratio in my opinion.

If I do not want to listen to something from my collection, I turn
myself towards YouTube Music. However, as I do not intent to financially support
Google by being imposed to watch or listen to ads or by paying a subscription
for what is not my main source of consuming music, I use hacked clients. On PC
I use the wrapper [YouTube Music Desktop][youtube-music-desktop] which blocks
ads but also brings in a lot of quality of life improvements such as native
media controls support and Discord Rich Presence integration. On mobile, I
obviously use [Vanced][vanced].


[art-companion]: https://github.com/tina-otoge/artcompanion
[webtorrent-cli]: https://github.com/webtorrent/webtorrent-cli
[mpv]: https://mpv.io/
[youtube-dl]: https://github.com/ytdl-org/youtube-dl/
[jellyfin]: https://jellyfin.org/
[gelli]: https://github.com/dkanada/gelli
[flood]: https://flood.js.org/
[youtube-music-desktop]: https://th-ch.github.io/youtube-music/
[vanced]: https://vancedapp.com/

## Flatpak, Flathub, and the joy of containerization

I used to not be a fan of application distribution solutions for Linux, as I
thought there was no point since repositories and package managers are already a
thing. This changed and I now know the benefits they have, and why
[Flatpak][flatpak] is the best among the competition.

Flatpak is a way to package and distribute applications for Linux, it is not
dependent on the Linux distribution used to run them, and uses containers
technology to run each app in its own isolated environment. Applications can be
installed either on a per-user basis or globally. The degree of isolation can
be configured for each application, providing a level of control similar to
what you are used to on Android.

![screenshot of flatseal](https://tina.moe/assets/cloud/blog/computer-tour-2022/flatseal.png)

This is very useful for many reasons, for example, if you do not entirely trust
an application, you can limit its access to the files on your system or revoke
its access to the Internet. This way the Chinese government won't be able to spy on
you. It is also useful if you do not wish to install the dependencies of an
application on your system. I had this with GIMP because I made the choice to
completely remove Python 2 from my computer, but GIMP still depends on it, so I
moved from the packages repository release to the Flatpak one. One last big
appeal of Flatpak is obviously for developers, as they can write their app and
target only one platform, the one used for their Flatpak release, it's way less
work than making sure their application works on every distribution.

[Flathub][flathub] is the main storefront for Flatpak applications, I already
showed how it can be integrated into the GNOME Software app earlier, it provides
a platform to publish and search applications.


[flatpak]: https://flatpak.org/
[flathub]: https://flathub.org/

## Other applications tour

There are a number of other applications I use I haven't talked about, and since
I use them every day and got so used to them, I kind of forget what really
sticks out and is worth recommending. First of all, here's a screenshot of my
application drawer.

![my application drawer](https://tina.moe/assets/cloud/blog/computer-tour-2022/gnome-drawer.png)

There are a bunch of developer tools in there, such as
[sqlitebrowser][sqlitebrowser] and [DBeaver][dbeaver], popular tools to interact
with databases, or the editors Vim and Neovim.

I use Firefox as my Internet browser and I like what Mozilla creates and does. I
however, also have ungoogled-chromium installed as I like one of the features
Chromium has, which is being able to run a website in a dedicated app-like view,
creating the illusion it is not running in a browser. I use that to run
Jellyfin, Mahjong Soul, or Taiko Web for example.

![majsoul in chromium's app mode view](https://tina.moe/assets/cloud/blog/computer-tour-2022/majsoul.png)
*Mahjong Soul running in Chromium's app mode, making it look like an actual
desktop application*

I use GNOME's default files explorer, Nautilus, even though I do most of my
file interactions directly through a terminal. It is still useful to have when
I want to do things such as accessing a network location, or browsing through
pictures like screenshots visually.

[Flatseal][flatseal] is the app I showed earlier to view and manage the
permissions of Flatpak applications. A must-have if you use Flatpaks because it
is very tedious to audit the permissions through the terminal.

I use GIMP to edit screenshots or make simple collages. I'm envious of some
features it lacks compared to Photoshop such as the smart magnets and attaching
effects to layers, but for my use cases, it's more than enough.

Finally, I use [virt-manager][virt-manager] to run virtual machines. I tried
GNOME's default option which is called Boxes, dumbs down the process of
setting up VMs to its simplest, and think it's good for people who just want to
try some OS quickly and easily. But I was quickly frustrated by the lack of
features. virt-manager offers everything I need, is simple enough to use, and
most importantly isn't made by Oracle.


[sqlitebrowser]: https://sqlitebrowser.org/
[dbeaver]: https://dbeaver.io/
[flatseal]: https://github.com/tchx84/Flatseal
[virt-manager]: https://virt-manager.org/

## What about Windows?

On Windows, I do not have any notable things. If anything, my Windows setup is as
simple as it can be as I use it exclusively if I want to play games or stream.

I hide the desktop icons from view (right-click on desktop, view > show icons).
I think the desktop looks way more beautiful without them. If I need to access
my files, Firefox or Discord, I use the keyboard shortcuts I mentioned (Windows
+ 1, 2, or 3) as they are the only things pinned to my status bar. For other
applications, I bring up the Start Menu with a single press on the Windows key
and then either type the name of an app or click in the list of applications,
just like I would do on Linux. My Start Menu is tidy enough to only contain
stuff I actually use.

I use ShareX, the very powerful screenshot tool which I often miss when I'm on
Linux. It allows for quickly editing your screen before snapping a picture,
such as adding texts or underlining and highlighting things. It also has a very
wide range of post-capture options, such as uploading to a hosting service,
tweeting, saving it in a local folder, copying to the clipboard, and more.

Some of the tools I use on Linux are also available on Windows, such as mpv,
youtube-dl, and WebTorrent. I could use Vim but the Windows distributions of it
are a pain to use, so instead, I use VS Code with the Vim extension. The YouTube
Music Desktop app is available too.

---

And I think that's pretty much it! That was a way bigger article than what I
envisioned, and I don't think I will have the energy to update it over time, so
you should not consider everything in it as a reference of what I still use if
you are reading this in a far future.

I really hope you were able to learn about tools you did not even know existed
before reading this, and that you will be able to improve your everyday computer
life by borrowing a thing or two from me!

If you have any questions about anything I talked about here, don't hesitate to
bug me on Twitter or Discord.
