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


## Templates
Contains template files for populating your file manager's "new file" or "create document" context menu.  

Nemo manages to include mimetype icons in its menu, which is nice.  
<img width="411" height="228" alt="image" src="https://github.com/user-attachments/assets/20d7d465-6c01-4e7a-8cfb-0ab205752f75" />


Not sure why a few basic ones aren't included in a default Linux installation. Also I've never seen this documented in an obvious place before, so unless you go googling for it, you probably don't know about it.  
