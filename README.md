[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

# GNTgreek2betacode

Repository detailing the process of converting Greek text to and from Betacode which is a necessary step for applying [Morpheus morphological tagging](https://github.com/perseids-tools/morpheus) to the Greek words in the [N1904-TF](https://centerblc.github.io/N1904/) dataset of the New Testament.

## Documentation

 - [Beta Code encoding](https://stephanus.tlg.uci.edu/encoding.php)

 - [Quick: TLG Beta Code Quick Reference Guide (pdf)](https://stephanus.tlg.uci.edu/encoding/quickbeta.pdf)

 - [Full: The TLG Beta Code Manual (PDF)](https://stephanus.tlg.uci.edu/encoding/BCM.pdf)

## Main notebooks

 - [Create NT wordlist in Betacode.ipynb](create_NT_wordlist_in_Betacode.ipynb): Create the wordlist from the N1904 corpus.

 - [Mapping unicode to betacode.ipynb](mapping_unicode_to_betacode.ipynb): The conversion from Unicode to Betacode.

## beta-code-py

The engine for these notebooks is [beta-code-py](https://github.com/perseids-tools/beta-code-py) which is available under the [MIT license](https://github.com/perseids-tools/beta-code-py?tab=MIT-1-ov-file). Hence these notebooks are also made available under the same license.

## Example usage beta-code library

Transcoding between beta- and uni-code you can easily be done in the following manner:

```python
import beta_code

beta_code.greek_to_beta_code(u'χαῖρε ὦ κόσμε')
'xai=re w)= ko/sme'

beta_code.beta_code_to_greek('xai=re w)= ko/sme')
'χαῖρε ὦ κόσμε'
```

## Online conversion between Beta- and Uni-code

An online conversion tool was developed by Zachary Fletcher and published in his repository [zfletch/beta-code-converter-js](https://github.com/zfletch/beta-code-converter-js). The tool is available for use online at [apps.perseids.org/beta-code](https://apps.perseids.org/beta-code/).

## Betacode feature for N1904-TF 

A new feature [`betacode`](https://github.com/tonyjurg/N1904addons) has been created that can be loaded as addtional module together with the [N1904-TF](https://centerblc.github.io/N1904/) Text-Fabric dataset of a syntactic anotated Greek New Testament.
