# Embedded display font

The website embeds a WOFF subset of Nimbus Sans Bold from URW Base 35.

Copyright 2015 URW Software; 2013, 2014 (URW)++ Design & Development.
The font is licensed under AGPL-3 with the font exception stated in the accompanying `COPYRIGHT.txt`. That notice contains the complete license text. These terms concern the font; no license for the user's portrait or personal content is granted here.

Source: https://github.com/ArtifexSoftware/urw-base35-fonts

Modification: on 2026-10-08, the font was subset to Unicode code points 32 through 126 and converted to WOFF for embedding. Its source OTF is included as `NimbusSans-Bold.otf`.

To reproduce the embedded subset, run the following in this directory after installing Python and `fonttools`:

```python
from fontTools.ttLib import TTFont
from fontTools import subset

font = TTFont('NimbusSans-Bold.otf')
subsetter = subset.Subsetter()
subsetter.populate(unicodes=range(32, 127))
subsetter.subset(font)
font.flavor = 'woff'
font.save('NimbusSans-Bold-subset.woff')
```

This is only a font-reproduction example; it is not needed to run or publish the website.
