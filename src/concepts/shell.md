# Command Line Interface (Shell)

  Today, you are probably most familiar with interacting with your computer via a **graphical user interface (GUI)**.

For example, how would you move a file called `notes.txt` from your desktop to a folder called `COMP401` that also resides on your desktop? In a _graphical_ user interface (and assuming you aren't using software like a screen reader), that operation would probably look something like:
- Navigate to your desktop
- Click on `notes.txt`
- Drag `notes.txt`, holding the mouse button
- Release the mouse button over the icon for the `COMP401` folder

Under the hood, the operating system understands those graphical operations and carries out the expected operations.

Long before the graphical user interface, however, came the **command line interface (CLI)**. Nowadays, operating systems still provide access to this text-based interface, but usually by way of a graphical application (e.g., the `Terminal` app on MacOS).

The term "shell" is often used to refer to this type of interface, and a shell is itself a category of software that exposes the outermost layer of the operating system. `bash`[^bash] is a commonly included shell software on Unix-like systems.
- In MacOS 10.14 and below, `bash` is included as the default shell. In 10.15+, an alternative (but popular) shell interface called `zsh`[^zsh] is the default instead. For basic functionality, they are effectively interchangeable.

In `bash` or `zsh`, the same operation as above (moving a file into a folder) could be achieved by running the following text commands:
```bash
cd ~/Desktop
mv notes.txt COMP401
```

- `cd ~/Desktop`
  - `cd` is the command to "change directory"
  - `~/Desktop` is the path to the destination directory
    - `~` in file path is widely-recognized shorthand for "the current user's home directory" (where the `Desktop` directory usually is)
- `mv notes.txt COMP401`
  - `mv` is the command to "move" something
  - `notes.txt` is the source file that we want to move
  - `COMP401` is the destination where we want the source file to end up

## Why not just use the GUI?
For this simple operation, using the GUI would be a perfectly reasonable solution. But...
- What if you needed to move files to different directories based on their name?
- What if you needed to parse the contents of the file and determine its destination based on the result?
- What if you knew some of the files could produce errors while trying to move them, and you wanted to handle those errors?
- What if these files were very important and you wanted to verify everything copied correctly?

These are all common situations to end up in as a software engineer and may already be familiar to you if you've ever written code. Once you're comfortable with it, working in the CLI enables you to automate tedious, complex operations by writing scripts that do the work for you.

Besides this, you can install a variety of powerful utilities, some of which are available solely in the CLI.

---
[^bash]: [What is bash?](https://opensource.com/resources/what-bash)

[^zsh]: [What is zsh?](https://zsh.sourceforge.io/FAQ/zshfaq01.html#l3)
