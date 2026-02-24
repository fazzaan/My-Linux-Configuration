# My Linux Configuration

## dconf 
Contains dconf keys.  

* .dconf files are entire directories from dconf.  

* .gsetting files are single keys from dconf.  
  _These are necessary when you only want one key. `dconf dump` doesn't have a method for this._ 🤷  

.dconf files were made using `dconf dump /org/path/ > file.dconf`.  
They can be imported using `dconf load /org/path/ < file.dconf`.  

.gsettings files were made using `gsettings get org.path > file.gsetting`.  
They can be imported using `gsettings set org.path key-name "$(cat file.gsetting)"`.
