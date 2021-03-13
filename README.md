# Mediainfo-Template
![ScreenShot](https://raw.githubusercontent.com/optio50/Mediainfo-Template/main/MediaInfo-Custom-Template.png?raw=true|alt=octocat)

Mediainfo Custom Template Example

This is a nicely formatted example of how to use the custom mediainfo "Inform" template.
After much searching due to the lack of Mediainfo documentation and frustrating examples
I have created a simple easy to read template.
All other examples I found seem to CRAM all the parameters on a single line makeing it difficult to read and understand.
You dont have to cram them all on one line if you quote the "Sections" from begining to end.
Also included is ALL parameter file. This file lists every available data type.
I was motivated to do this because I am of the opinion that the "Encoding settings" takes up way too much space and makes
an otherwise nicely formatted output look cluttered and ugly.
This template omits that section.

Commandline Example
mediainfo --Inform=file:///Path/To-File/Inform-Example.txt 'Blue Planet II - S01E02 - The Deep.mkv'
