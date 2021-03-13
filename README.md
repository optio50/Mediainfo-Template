# Mediainfo-Template
![ScreenShot](https://raw.githubusercontent.com/optio50/Mediainfo-Template/main/MediaInfo-Custom-Template.png?raw=true|alt=octocat)

Mediainfo Custom Template Example

This is a nicely formatted example of how to use the custom mediainfo "Inform" template.  
After much searching due to the lack of Mediainfo documentation and frustrating  
examples I have created a simple easy to read template.
All other examples I found seem to CRAM all the parameters on a single line making it difficult to read and understand.  
You dont have to cram them all on one line if you quote the "Sections" from begining to end.  
Also included is ALL parameter file. This file lists every available data type.  
I was motivated to do this because I am of the opinion that the "Encoding settings" takes up way too much space and makes  
an otherwise nicely formatted output look cluttered and ugly.  
This template omits that section.

Commandline Example  
```mediainfo --Inform=file:///Path/To-File/Inform-Example.txt 'Blue Planet II - S01E02 - The Deep.mkv'```

Some data are blank due to the file not having that info.
If your file has no information for the "Section", the entire section will be seemlessly omitted.
Works equally well with Video and Audio files.

I am still uncertain about a few things.
For instance.
In the standard regular output of Mediainfo if a value is null it is conveiently removed / deleted.
I can only come close to replicating this "$if(%Value%)" but a blank line is still printed (undesirable).
Until I figure this out I have not included it.

I am also unsure about the examples that include
```
File_Begin;
File_End;
Page_Begin;
Page_Middle;
Page_End;
General_Begin;
General_End;
Video_Begin;
Video_Middle;
Video_End;
Audio_Begin;
Audio_Middle
Audio_End
Text_Begin
Text_Middle
Text_End
Chapters_Begin
Chapters_Middle
Chapters_End
```
I beleive this is for HTML table formatted output on where to place the output.

Mediainfo standard output can also display chapter information.
Such as.
```
Menu
00:00:00.000                             : :Chapter 1
00:06:40.640                             : :Chapter 2
00:11:49.680                             : :Chapter 3
00:16:50.680                             : :Chapter 4
00:22:16.800                             : :Chapter 5
00:25:59.400                             : :Chapter 6
00:29:58.200                             : :Chapter 7
00:36:46.760                             : :Chapter 8
```
A recent post by the developer indicated this is not available in the INFORM custom template.
