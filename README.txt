This is here since we inevitably won't remember how to configure anything. clone this into ~/.config, so it will look like ~/.config/nvim
1. Open neovim and run :PackerSync
2. Run :PackerInstall
3. Run :PackerUpdate
4. Keep doing steps #1 #2 #3 until it works better

For nerdfonts (so that nerdtree doesn't look terrible):
1. Go to a link with nerdfonts like: https://github.com/ryanoasis/nerd-fonts/releases
2. Download the tar or zip for whatever font you want. I did the 3270 tar since who really cares what the font is
3. Extract the contents to wherever, probably just Downloads
4. Run the following:
cd ~
mkdir -p ~/.fonts
mv path/to/extracted-fonts/*.ttf ~/.fonts/
fc-cache -fv

For live grep in telescope run the following in a terminal:
sudo apt install ripgrep

If you already have neovim configurations installed and are getting issues then do this:
1. sudo apt remove --purge neovim
2. rm -rf ~/.config/nvim/
3. rm -rf ~/.local/share/nvim/
4. rm -rf ~/.local/state/nvim/
5. find / -name "*nvim*" 2>/dev/null
Then reinstall neovim and try again. 

