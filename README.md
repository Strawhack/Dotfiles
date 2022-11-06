# Dotfiles
My Configuration for Vim and Tmux


### ToDo For Tmux

#### Install Xclip
```sh
$sudo nala -y install xclip    (If Nala is installed)

$sudo apt -y install xclip     (Using apt)
```

#### Install Font-Manager
```ruby
$sudo nala install -y font-manager

Download Meslo Font 
https://github.com/romkatv/dotfiles-public/tree/master/.local/share/fonts/NerdFonts

Install Fonts using font-manager
```

#### Configure Tmux
```sh
Create .tmux.conf file
$touch ~/.tmux.conf

Paste the content from tmux dotfile in ~/.tmux.conf

save the file
$tmux source ~/.tmux.conf
```

#### Install Plugins for Tmux
```python

Git Clone the below Link
$ git clone https://github.com/tmux-plugins/tpm.git ~/.tmux/plugins/tpm

Edit ~/.tmux.conf
set -g @plugin “tmux-plugins/tpm”
set -g @plugin “tmux-plugins/tmux-sensible”

# Dracula Theme
set -g @plugin 'dracula/tmux'

# available plugins: battery, cpu-usage, git, gpu-usage, ram-usage, network, network-bandwidth, network-ping, weather, time
set -g @dracula-plugins "cpu-usage ram-usage time"
set -g @dracula-show-powerline true
set -g @dracula-show-timezone false
set -g @dracula-day-month true

# Initialize TMUX plugin manager (keep this line at the very bottom of tmux.conf)
run “~/.tmux/plugins/tpm/tpm”

Save the File.

To Activate Theme
1. Run tmux
2. Ctrl + A + I
```
