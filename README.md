# Playbook template

Developed by Rasmus Aagaard (s164419) in 2019 and further developed by Niels Kjær Ersbøll (s183903) in 2020 based on and inspired by the template created by Henriette Steenhoff (s134869) in 2015

Link to a read-only version of the template can be found on [Overleaf](https://www.overleaf.com/read/ykxbtwyfnyzv)

## General information about the template

In this template you will find a lot of specific things created for the rustrips. The template only exists as a guide and you should of course thoroughly it through and edit it to fit your timestamps, distrubution of responsibilities etc.

## Code names

Codenames are specified by the command `\codename` which takes 3 parameters: the name itself (what you want to write to show it), the colour and the name. Example: `\codename{\DAK}{orange}{Dr Dakkensmirtz}`

All available colours are taken from [latexcolor.com/](http://latexcolor.com/)

## Contact information

Fill out `latex/front_matter/contactinfo.tex` with relevant infromation from [Studiestartswikien](https://studiestartswiki.pf.dk/en:rusturshytter:start). You could even take inspiration from previous playbook which should be available at the bottom of the page for the cabin (might not include english playbooks).

## Timetable

An example for a timetable can be found in the fle `latex/days/01_arrival/01_timetable.tex`. To inserting multitple lines in the timetable one can with advantage place the cursor on a line in the timetable and hold down the buttons `Shift+Alt` and press either up or down on the keyboard arrows. This will copy the actual line.

## Material list

When making the material list we use commands from the file `matlist.tex` which can be found in `latex/settings/matlst.tex`. You start by creating the `mats`-enviroment (`\begin{mats}{}{}`) and write the date and activity. Example: `\begin{mats}{Saturday}{Bustrip}`. After this you list each material by writing `\mat{}{}`, the parameters of which indicates quantity and material. Example `\mat{750}{Glowsticks}`. Examples of this can be found in the playbook. `matlist.tex` collects all materials at the end of the playbook. This makes it easier to identify which materials to use which day and for which activities.
