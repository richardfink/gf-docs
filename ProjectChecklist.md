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

