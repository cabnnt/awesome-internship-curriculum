# Operating System
The operating system bridges the gap between the applications that run on a computer and its hardware. Microsoft Windows, MacOS, and Ubuntu (a particular distribution of Linux) are all common examples of operating systems.

When writing high-level[^programming-language-level] programming languages (e.g., Ruby, JavaScript), you will (by design) rarely need to think about your underlying hardware and the implementation of the underlying operating system. More low-level[^programming-language-level] languages (e.g., C) still communicate with the operating system, but generally require more direct interaction with the hardware (e.g., manually allocating/de-allocating memory).

Even if you are working exclusively with high-level languages, it's useful as a developer to be familiar with the basics of navigating, manipulating files, and running applications via the command line.

## Unix-like (or *nix)
For historical reasons, many[^server-market-share] of the servers you will encounter and interact with on the web are based on a "Unix-like"[^unix-like] operating system. These operating systems typically provide a common interface via a "shell" or command line, which we'll cover in the next section.

- If your computer is running **MacOS** or any **distribution of Linux**, you're already using a Unix-like operating system.
- If your computer is running **Microsoft Windows**, your operating system is not Unix-like. You can setup a Linux distribution "within" Windows via [Windows Subsystem Linux (WSL)](https://docs.microsoft.com/en-us/windows/wsl/install).

---
[^programming-language-level]: [High- and low-level programming languages](https://en.wikipedia.org/wiki/High-_and_low-level)

[^server-market-share]:
  [Share of servers on the web by operating system](https://en.wikipedia.org/wiki/Usage_share_of_operating_systems#Public_servers_on_the_Internet)

[^unix-like]:
  [Unix-like operating systems](https://en.wikipedia.org/wiki/Unix-like)
