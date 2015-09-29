# Introduction

This page lists how to learn enough about Git to move an open font project available in this Mercurial repository to a Git repository, and how to manage a open font project with it.

## Project Repository

- [ ] Set up a Github Repo

New to Git and Github? Play the http://try.github.io 15 minute interactive game, and read http://nvie.com/posts/a-successful-git-branching-model, an essay about using Git for ongoing project management.

- [ ] README.md file

Each Github repo must have a README.md that summarises the project. This may include

- [ ] DESCRIPTION.en_us.html

Description paragraph to be used in font directories.

- [ ] BRIEF.md

Each Github repo must have a BRIEF.md that describes the project. 

- [ ] Actual source files

Your project will include _actual_ source files, the ones that you use yourself when drawing the design. 
These are often quite 'messy', but no problem. 
Often these are Glyphs files, sets of UFOs, VFBs, or SFDs.

- [ ] Build source files

You may maintain a set of 'build sources', which are updated less frequently than the actual source files, and updated with care. 
They may have some 'pre-build' operations applied, like Remove Overlaps, and are used as input to a build script. 

- [ ] Build script 

You may maintain a build script that runs the build steps, or you may make a tutorial for taking those steps manually (or a mix.)

- [ ] Binary files
 
After the build process you will have OTF and TTF files.

- [ ] "Clean" repo

There should not be 'stray' files in the repo, such as `.empty` 

## Production

- [ ] Including ttfautohint 
- [ ] Including ttfautohint controls file

## Latin Design

- [ ] Support the 219 "base Latin" glyphs https://github.com/google/fonts/blob/master/tools/encodings/latin_unique-glyphs.nam
- [ ] Support Adobe Latin 3 http://adobe-type-tools.github.io/adobe-latin-charsets/adobe-latin-3.html
- [ ] Support Adobe Latin 4 (mainly Vietnamese) http://adobe-type-tools.github.io/adobe-latin-charsets/adobe-latin-4.html
- [ ] `.notdef` glyph is a recommended design https://www.microsoft.com/typography/otspec/recom.htm
- [ ] Anchors for all letter and diacritics https://github.com/weiweihuanghuang/Work-Sans/pull/17#issuecomment-139910842

## OpenType

- [ ] Support Turkish with OpenType http://typedrawers.com/discussion/1101/izmir-turkey
- [ ] Support tabular numbers across the family http://typedrawers.com/discussion/1103/tabular-figures-width-consistency#latest

## Test Documents

- [ ] http://understandingfonts.com/2011/fonttest
- [ ] http://impallari.com/testing
- [ ] http://testmyfont.com

### Tests

- [ ] Test for all letter/diacritic combinations https://github.com/weiweihuanghuang/Work-Sans/pull/17#issuecomment-139910842



# Further reading

### UFO

The UFO format is documented at http://unifiedfontobject.org and developed on Github (https://github.com/unified-font-object/ufo-spec) and the ufo-spec mailing list (https://groups.google.com/forum/#!forum/ufo-spec)

## Proposed Changes By Richard Fink

1) It seems to me that the brief.md is the most important file in the repository. And it seems smart to me for the Google fonts team to be the ones to contribute the brief.md file which describes the project and the contents of the repo. Asking the contractor to describe the requirements seems odd to me. It seems upside down. They are font designers, not technical writers and/or project managers. What's needed is a clear summary of the work being commissioned by those who are commissioning or did commission it. This way, it becomes a reference and a guide, not only to anybody who forks the contents of the repo for whatever reason, but to the original contractor(s)! And, once they've read it, if there is anything in it that doesn't seem right, well, the time to clarify is at the beginning of the project, not the end. Their job is making the fonts and making them right. But I've designed production systems on the factory floor, Dave, and a clear statement of what's expected is crucial. People need to know exactly what it is they are supposed to do. Over the next few days I'm going to spend a little time reading over the GFD reports from some of the contributors whose work I haven't at all reviewed and see what they have to say.
It seems to me that it shouldn't be left up to the contractor to produce a summary of what they are being asked to live up to. needed is a statement of what IS the job. This way, if anything substantial goes amiss, the phrase "Check the brief.md for clarification on that" can, and should be, the mantra. (And somewhere in the brief.md file it should make it clear that things need to be done in accordance with the projectchecklist.md.)

2) There are certain technical requirements that we've seen come up with the Cadson Demak fonts and a subchecklist of those requirements within the projectchecklist.md should be started. It's "best practice" stuff for webfonts, that's all. 
Stuff like:
1) The embedding bit set to 0. 
2) Vertical Metrics done right.
3) Empty and stray tables. (We've discussed the empty DSIG tables but there are some others to take into account also. The inner structure of the font is important.)
4) The correct setting for the gasp table. 
5)   ---  more to come ----
