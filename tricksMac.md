Awesome Terminal Tips & Tricks for Mac Users
===============================================

# Create An Alias for a command

With Terminal, you can create an alias for a command.

As an example, let’s create an alias surf that opens up medium.com. To open up medium.com via Terminal you need to use open [URL] syntax:

open https://www.medium.com

To create an alias surf for this command:

    Open up your .bash_profile:

open ~/.bash_profile

1. Create a new alias surf by adding the following into the .bash_profile:

alias surf='open https://www.medium.com'

2. Save the file and restart Terminal.

3. Now type in surf and medium.com opens up in the default browser.

# Show Your Command History

View your Terminal command history by typing history in Terminal.

# Easily Find Forgotten Commands from History

This is the one I use a lot. It’s is a time saver when there is a complex command you’ve run some time ago and you cannot remember/find it.

To find earlier commands from your Terminal’s history:

    Open up Terminal.
    Type Ctrl-R.
    Start typing (e.g. letters you remember from the command you’re searching for).
    As you type, the terminal keeps suggesting a command that matches what you’ve typed. To execute the suggested command, hit enter.

# Show Hidden Files and Folders

To show hidden files and folders, type these two commands:

defaults write com.apple.finder AppleShowAllFiles -bool TRUEkillall Finder

Be careful with the hidden files. There is likely a reason why they are hidden by default. Do not delete anything you are not sure you want to delete.

To hide these files back, run the above commands by replacing TRUE with FALSE.

# Copy-Paste Files from Folder to Another

Use ditto to copy and paste files from a folder to another. The general syntax is:

ditto [original_folder][new_folder]

For example, if you have a folder called folder1 and you want to create a new folder, folder2, and copy-paste the contents of folder1 there, just type:

ditto folder1 folder2

# Download Without Browser

If you don’t want to use the browser to download a file, Terminal can help.

Before downloading with Terminal, notice that the downloaded file will end up in the directory where you currently are. So if you want it to end up in the Downloads, change directory there before downloading:

cd ~/Downloads/

To download the file, use cURL -O [URL_OF_THE_FILE].

For example:

curl -O https://www.medium.com/example_download.txt

# Keep Your Mac Awake

To disable your Mac from falling asleep, just type:

caffeinate

To stop caffeinating, just type Ctrl-C.

To caffeinate for a period of time use caffeinate -u -t [num_seconds]. For example, let’s caffeinate for 10 minutes (600 seconds):

caffeinate -u -t 600

(Naturally, this can be escaped with Ctrl-C too.)

# Repeat Characters by Holding Down a Key

Holding a key to repeat characters is something most of us are used to. Luckily, there is a way to enable it in Mac using Terminal:

defaults write -g ApplePressAndHoldEnabled -bool FALSE

To undo this, run the above command and replace FALSE with TRUE.

# View Contents of a File Without Opening It

Use cat [path_to_file] to view the contents of a file without opening it.

For example, say you have a python file example.py in your current directory and you want to check its contents with Terminal.

To achieve this, just type:

cat example.py

# Make Your Mac Speak

Use say [what_to_say] command to make your Mac speak.

For example, to make your Mac say Hello, World!, run the following command:

say Hello, world!

Bonus Trick—ASCII Art

To display ASCII art text, use this syntax:

banner -w [banner_width][banner_text]

As an example, let’s print "Hello" as below:

banner -w 50 Hello

