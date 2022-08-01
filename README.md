# Playbook template
Made by af Rasmus Aagaard (s164419) in 2019, translated by Rasmus Sundin (s196677) and Jonathan Højlev (s194684) in 2022 with inspiration from a template made by 
Henriette Steenhoff (s134869) in 2015.

Link to non-editable version of the tamplate can be found here: [Overleaf](https://www.overleaf.com/read/bnvybpjpthgq)

## Short introduction to the template

You can in this template find a lot of things that is specific to the rustrip that the template was made for. You should of course read it through yourself and edit so that it fit your trip. 

## Namecodes
Namecodes is given with the command Namecodes and is given by the command `\namnecode` which takes three parametres: the namecode itself, , Ie. the thing you want to you want to write to make the namecode appear in the playbook, the colour and the name. For example 
`\navnekode{\DAK}{orange}{Dr Dakkensmirtz}`.

All colours to the namecodes are taken from [latexcolor.com/](http://latexcolor.com/)

An idea could be to give the teams a namecode that is their crossvector's namecode, just with reverse big/small letters, so for example if the vector's namecode is `\MEME` will the team's name be `\meme`, or reverse.
Input from Rasmus Sundin, another idea could be to make a namecode so that if it the vector's name, for exmple Dr. Dakkensmirtz use `\navnekode{\DAK}{orange}{Dr Dakkensmirtz}`, but if you want to mention the team make a namecode`\navnekode{\DAKC}{orange}{Phineas and Ferb}` where the C stands for crossteam assuming Phineas and Ferb was the vector's teamname. 


## Contactinformation
Fill out`latex/front/contactinfo.tex` with relevant information from [Studiestartswikien](https://studiestartswiki.pf.dk/rusturshytter:start). Take inspiration from old playbooks, they can be found in the bottom on the page for your cabin. 

## Timeschedule
You can find an example on a timeplan in the file `latex/dage/01_ankomst/01_tidsplan.tex`. To insert more lines in the timeplan can you put your mouse on the line in the timetable, tap `Shift+Alt`and tap on the up or down keys on the keyboard. This will copy the line. 

## Materialslist
For making the materialsslist use the file `matlist.tex` which can be found in `latex/settings/matlist.tex`. To use this you use `mats` like this;  (`\begin{mats}{}{}`) and from there give day og activities, for example `\begin{mats}{saturday}{bustrip}`. Thereafter can you give the material and the quantity using `\mat{}{}`, where the parameters is the quantity and and the material, like this; `\mat{750}{glowsticks}`. Example of this can be found here and there in the playbook. `matlist.tex` Will show all materials that have been written in with the format mentioned earlier, creating an easy overview of the materials needed, the quantity and whn. 

## How to make the materiallist fit into one page
There will often be very long tables, that there will not be space for on one page. Here you can use `\begin{landscape}` to flip the page to be horizontal instead of vertical. 

