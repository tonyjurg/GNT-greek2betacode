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

The engine for these notebooks is [beta-code-py](https://github.com/perseids-tools/beta-code-py) which is available under the [MIT license](https://github.com/perseids-tools/beta-code-py?tab=MIT-1-ov-file). Hence these notbooks are also made available under the same license.
