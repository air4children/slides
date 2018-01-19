LOGBOOK
---


# TODO LIST

- [ ] Choose the right resolution for images to present the logos in the background image for the \maketitle and \closingtitle
  __(CREATED:19january2018, SORTED:: commit: [0000](0000) )__

- [ ] organise the references, maybe add bibtex file
  __(CREATED:19january2018, SORTED:: commit: [0000](0000) )__


# SORTED LIST

- [x] Create background for the \maketitle and \closingtitle
  __(CREATED:9JANUARY2018, SORTED:19january2018: commit: [0000](0000) )__

- [x] add references
  __(CREATED:20DEC2017, SORTED:19january2018: commit: [0000](0000) )__


# CHANGES IN THE TEMPLATE OF THE PRESENTATION


- [x] Makefile has been modified to decrease the resolution of images therefore their size
```
%.png: %.svg
         inkscape --export-png $(@) $(<)
```
	__(19january2018)__

- [x] Fix the size of the black background and legend background on each image by changing at /style/beamerthemehri.sty
```
rectangle/.style={fill=hriBlack}, show background rectangle]
\node at (-1, -4.5) [anchor=south west,shape=rectangle,fill=hriSec3Blue, opacity=0.8, align=left, text width=0.6\paperwidth]
```
and using  http://latexcolor.com/ to set colors for background
```
\definecolor{hriSec3Blue}{rgb}{0.0, 1.0, 0.0}
```
  __(CREATED:20DEC2017, SORTED:9JANUARY2018: commit: [0000](0000) )__
