# sync_git

This is the repository I use to synchronize data accross multiple computers.
The actual data is stored in a git repository contained in "encrypted"---a veracrypt disk.
Thus, I'm effectively using this like a google-drive style thing.
Go figure.

I make no guarantees about anything in this repository. Use at your own risk.

# Scripts

Use this git_config script to do initial set up (adding the correct remotes and possible ssh key set up).
Use mount and umount to respectively mount and unmount the encrypted disk.
Use push_remotes to push to all remotes.
Use pull_remotes to ensure the remotes are synchronized and then pull arbitrarily from one of them.
Use verify_remote

# Dependencies

The scripts were developed with the following tools. Other versions may work, but have not been tested.
- bash 4.4.12 (all scripts)
- git 2.15.1 (git_config, push_remotes, verify_remotes, pull_remotes)
- OpenSSH 7.4 (git_config)
- veracrypt 1.21 (mount, umount)

In addition, verify_remotes uses the POSIX tools wc and uniq.
