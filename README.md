## Command and Conquer
- [Presentation slides](https://jonoliver.github.io/command-and-conquer/)
- [Oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
- [My dotfiles](https://github.com/jonoliver/dotfiles)


### Resources

#### Dotfiles
- https://dotfiles.github.io/
- http://blog.smalleycreative.com/tutorials/using-git-and-github-to-manage-your-dotfiles/

#### Tmux
- [Tmux cheat sheet](https://gist.github.com/MohamedAlaa/2961058)
- [Tmuxinator](https://github.com/tmuxinator/tmuxinator)
- https://pragprog.com/book/bhtmux/tmux

#### Remote Pair Programming
- http://pivotallabs.com/how-we-use-tmux-for-remote-pair-programming/
- http://www.pairprogramwith.me/
- [$10 credit at Digital Ocean](https://m.do.co/c/da72a8bfea8d)

#### Terminal Improvements
- http://iterm2colorschemes.com/
- https://mosh.org/

### Commands and Functions

```bash
# file manipulation

# create file
touch file_name

# remove file
rm file_name

# move file (or directory)
mv old_dir/file new_dir/file

# rename file (or directory)
mv old_file_name new_file_name


# directory manipulation

# create directory
mkdir dir_name

# remove (empty) directory
rmdir dir_name

# remove (non-empty) directory
# be careful with this one!!!
rm -rf dir_name

# creating an alias
alias pro='cd ~/Documents/projects'

# searching aliases
alias | grep "search term"

# searching history
history | grep "search term"


# fun with functions!

# make a directory and cd into it (works recursively)
mkcd() { mkdir -p "$@" && cd "$_"; }

# same as above, but also intialize git repo
new(){ mkcd $@ && git init }


# tmux

# create new tmux session
tmux new

# create new tmux session (with name)
tmux new -s "session_name"

# list tmux sessions
tmux ls

# attach to tmux session
tmux attach -t "session_name"

```

### Terminal emulators for Windows:
- [cmder](http://cmder.net/)
- [PuTTY](http://www.putty.org/)
- [Git for Windows](https://git-scm.com/downloads)
- [Cygwin](https://www.cygwin.com/)
