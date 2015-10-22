

Linux:

1. In your home directory if a ".vim" directory doesn't exis, then make one.

2. In your home directory, execute the command below:

       git clone --recursive https://github.com/michaelmoore44/vim-config.git .vim

3. Create a file named .vimrc, and add the following line to the file:

       source ~/.vim/config/vimrc

Windows:

1. I have vim installed in my Users directory in a folder named "vim" eg:

       C:\Users\moorem\vim

3. The easiest way to do this is to start with nothing in your vim directory
   except for your vim folder containing all the executables eg. "vim73". 

2. In whatever directory vim is installed in execute the command below:

       git clone --recursive https://github.com/michaelmoore44/vim-config.git vimfiles

4. Create a file named "_vimrc" under the vim install directory, and add the following
   line to the file in a form that is compatible with your setup:

       source C:\Users\moorem\vim\vimfiles\config\vimrc

       or:

       source $HOME\vimfiles\config\vimrc

   At work, my home directory is on a network drive, so I need to give the
   exact path of my vimrc file because I don't want to store it on the network.
   At home, I can use a variable like $HOME in the path to my vimrc file.

Add new package by navigating to the submodules directory and executing the
   command below:

   git submodule add <repo URL>

Generate helptags with :Helptags

