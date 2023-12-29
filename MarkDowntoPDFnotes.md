# Markdown to PDF

I wanted a pdf cover letter to upload that would link back to the markdown samples
I created here.  In order to get one that looked nice, I had to use the following 
process which I document here in case I need to reproduce an edited PDF later.

```
pip3.9 install grip
grip README.md
navigate to localhost:XXXX address
save html
search/replace the localhost:XXXX links back to github.com
edit the README.md heading to link back to github
open saved README.md.html in firefox
CMD-p
Choose print to file in the printer name dropdown
Choose scale and lower it until the whole page shows
Click save! 
```
