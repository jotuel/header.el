## header for emacs

###  Install using the script :

```bash
git clone https://github.com/jotuel/header.el.git
cd header.el
./set_header.sh workerbee bzzZZz@student.hive.fi         # usage :  ./set_header.sh [LOGIN] [MAIL]
source ~/.zshrc
cd ..
rm -rf 42header_emacs
```

Header shortcut (C - C H) is now functional.


### Manual install :
1) Copy all files in folder ~/.emacs.d

2) Change user-login and user-email var in file "header.el"   
   -> optional :    
      	  1/ Creating an env variable. In ~/.zshrc or ~/bashrc add the folowing command :   
            export HEADER42_LOGIN="yourlogin"  
            export HEADER42_MAIL="yourlogin@student.42.fr"  
	  2/ And run source ~/.zshrc or source ~/.bashrc to reload the source file
   	  
3) Header shortcut (C - C H) is now functional.

### Recommendation

Install Doom Emacs and `mv *.el ~/.config/doom/` + add following lines:
```
(load! "list.el")
(load! "string")
(load! "comments.el")
(load! "header.el")
```
to `config.el`. Run `doom sync` && enjoy.
