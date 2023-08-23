# Commands to know
Directory - Folder
CLI - Command Line Interface
Terminal - Interface for text commands
cd - Directory change
Repository - place or folder our project is kept
Github - WEbsite in which all projects are hosted
clone - To bring projects from GitHub to the local machine
add - Track files and changes in git
commit - save files in GIT
push - Commit to github
pull - pull down changes from GitHub to local machine

# Making your machine as a local machine to clone

### Generation of SSH keys 
Generating SSH keys involves creating a pair of cryptographic keys that can be used to authenticate you as an authorized user when connecting to a remote server via SSH. One key is kept secret and is stored on your machine (private key), while the other is shared with the remote service (public key).

#### Check for existing SSH keys: Before generating a new SSH key, you may want to check if you already have one.
``` GIT
ls -la ~/.ssh
```

Look for files named id_rsa and id_rsa.pub. If they exist, you already have an SSH key pair and don't necessarily need to generate a new one.

Generate a new SSH key pair: Run the following command, replacing "your_email@example.com" with your actual email address that you use for GitHub or whichever service requires the key.

bash
Copy code
ssh-keygen -t ed25519 -C "your_email@example.com"
Note: You can also use RSA keys instead of Ed25519 by running ssh-keygen -t rsa -b 4096 -C "your_email@example.com".

Save the key: When prompted to "Enter a file in which to save the key," press Enter to save it to the default location, usually ~/.ssh/id_ed25519 or ~/.ssh/id_rsa.

Set a passphrase: For added security, set a passphrase when prompted.
