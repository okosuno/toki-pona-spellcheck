### what

this is a spellfile which provides spellcheck for toki pona, [ISO 639-3 tok](https://iso639-3.sil.org/code/tok), in neovim or vim.  
[toki pona](https://tokipona.org/) is a constructed language with thousands of active speakers.  
in 2021 nearly one thousand speakers responded to a [community census](https://tokiponacensus.github.io/results/).  

### can i see?

![tokiembed](https://imgur.com/uaRGset)

### how do i use it?

this is how i did it.  
make sure your .vimrc has `set spell spelllang=tok,[other language codes]`.  
put the files (specifically `tok.utf-8.spl`) into `~/.local/share/nvim/site/spell/`.  
open nvim.  
you can now spellcheck in toki pona!  

### what words does it have?

everything on [lipu linku](https://lipu-linku.github.io/).  
this includes pu, nimi ku suli, and nimi ku lili.  

### what if i want to add/remove words?

make sure your .vimrc has `set spell spelllang=tok,[other language codes]`.  
put `tok.utf-8.add` into `~/.local/share/nvim/site/spell/`.  
modify the `tok.utf-8.add` file as desired.  
navigate to the location of the spell file and open neovim.  
enter `:mkspell! tok.utf-8.add`.  
you should see something like this output:  

```
Reading word file /home/[user]/.local/share/nvim/site/spell/tok.utf-8.add...
Compressing word tree...
Compressed case-folded of 1438 nodes; 691 (48%) remaining
Compressed keep-case of 18 nodes; 18 (100%) remaining
Writing spell file /home/[user]/.local/share/nvim/site/spell/tok.utf-8.add.spl...
Done!
Estimated runtime memory use: 3555 bytes
```

rename `tok.utf-8.add.spl` to `tok.utf-8.spl`.  
open neovim again.  
you can now spellcheck in toki pona!  

### you made a mistake!

yes, i make a lot of those.
you're welcome to contact me at [mi@okos.uno](mailto:mi@okos.uno) to help me fix it.
thank you for caring!
