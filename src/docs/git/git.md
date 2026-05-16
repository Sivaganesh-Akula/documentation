# Git

As you learn Git, try to clear your mind of the things you may know about other VCSs, such as CVS, Subversion or Perforce. Even though Git’s user interface is fairly similar to these other VCSs, Git stores and thinks about information in a very different way.

## Local VCS

Simple database thatkept all the changes to files under revision control. One of the most popular VCS tools was a system called RCS

## Centralized Version Control Systems

To deal with collaboration with developers problem, Centralized Version Control Systems (CVCSs) were developed

## Distributed Version Control Systems

This is where Distributed Version Control Systems (DVCSs) step in. In a DVCS (such as Git, Mercurial or Darcs), clients don’t just check out the latest snapshot of the files; rather, they fully mirror the repository, including its full history.

## Snapshots

- Conceptually, most other systems store information as a list of file-based changes. These other systems (CVS, Subversion, Perforce, and so on) think of the information they store as a set of files and the changes made to each file over time (this is commonly described as delta-based version control).
- Git doesn’t think of or store its data this way. Instead, Git thinks of its data more like a series of snapshots of a miniature filesystem. With Git, every time you commit, or save the state of your project, Git basically takes a picture of what all your files look like at that moment and stores a reference to that snapshot.

## Git Intigrity

Everything in Git is checksummed before it is stored and is then referred to by that checksum. The mechanism that Git uses for this checksumming is called a SHA-1 hash. This is a 40-character string composed of hexadecimal characters (0–9 and a–f) and calculated based on the contents of a file or directory structure in Git.

## Git States

- **Modified** means that you have changed the file but have not committed it to your database yet.

- **Staged** means that you have marked a modified file in its current version to go into your next
  commit snapshot.

- **Committed** means that the data is safely stored in your local database.

## Git setup

Git comes with a tool called git config that lets you get and set configuration variables that control all aspects of how Git looks and operates.

- `[path]/etc/gitconfig` file: Contains values applied to every user on the system and all their repositories. If you pass the option `--system` to git config, it reads and writes from this file specifically.

- `~/.gitconfig or ~/.config/git/config` file: Values specific personally to you, the user. You can make Git read and write to this file specifically by passing the `--global` option, and this affects all of the repositories you work with on your system.

- `config` file in the Git directory (that is, `.git/config`) of whatever repository you’re currently using: Specific to that single repository. You can force Git to read from and write to this file with the `--local` option
