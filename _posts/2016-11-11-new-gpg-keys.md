---
categories:
- hactivismo
- human rights
tags:
- pgp
- email security

header:
  overlay_image: /assets/images/scott-webb-lnRPKo7Lo5Q-unsplash.jpg
  teaser: /assets/images/scott-webb-lnRPKo7Lo5Q-unsplash.jpg
  caption: "CC0 Scott Webb / Unsplash"

excerpt: I am transitioning both my professional and personal GPG keys.
title: New GPG Keys!
created: 1478892596
---
I am transitioning both my professional and personal GPG keys. This transition document (in full, below) and both updated keys are signed with both old and new keys for both personal and professional accounts to validate the transition.

In short:
jcamfield@internews.org - new keyID <a href="https://sks-keyservers.net/pks/lookup?op=get&search=0xB46A01C3270C17F1">270C17F1</a>
jon@joncamfield.com - new keyID <a href="https://sks-keyservers.net/pks/lookup?op=get&search=0xDA9C4363FDDB8C25">FDDB8C25</a>

If this is all greek to you, GPG (or PGP) is a way to encrypt your email so that only other specific people (who must also be using GPG) are able to read it.  While we think of email like regular mail, with a level of privacy like something in an envelope, the reality is that it's better to compare it to a postcard.  If you're interested in getting started, I highly recommend EFF's excellent <a href="https://ssd.eff.org/en/module/introduction-public-key-cryptography-and-pgp" target="_blank">PGP guide</a>, and <a href="https://www.mailvelope.com/" target="_blank">Mailvelope</a> is a super-easy browser plugin to help get you started in more secure webmail (it works great, for example, with gmail).

<pre>
-----BEGIN PGP SIGNED MESSAGE-----
Hash: SHA256


Key Transition

I am transitioning both my professional and personal GPG keys. This transition document and both updated keys are signed with both old and new keys for both personal and professional accounts to validate the transition.

In short:
jcamfield@internews.org - new keyID 270C17F1
jon@joncamfield.com - new keyID FDDB8C25

Details follow:

PROFESSIONAL (jcamfield@internews.org, jon@openinternetproject.org)

The old key, which I am transitioning away from, is:

  pub   4096R/F926BF8B 2013-01-23
      Key fingerprint = 0020 1A37 47C0 0DEA C368 BCA5 A998 959F F926 BF8B

The new key, to which I am transitioning, is:

  pub   4096R/270C17F1 2016-11-11 [expires: 2018-11-11]
      Key fingerprint = D776 2A79 A1AE F000 7F53 A127 B46A 01C3 270C 17F1

To fetch the full new key from a public key server using GnuPG, run:

  gpg --keyserver keys.gnupg.net --recv-key 270C17F1

PERSONAL (jon@joncamfield.com)

The old key, which I am transitioning away from, is:

  pub   1024D/B10D0440 2006-04-05
      Key fingerprint = 3087 315E A392 4F9B 71A5 702D 2824 391E B10D 0440

The new key, to which I am transitioning, is:

  pub   4096R/FDDB8C25 2016-11-11 [expires: 2018-11-11]
      Key fingerprint = CEEB 0184 2F5B 923D 1CA0 BFCB DA9C 4363 FDDB 8C25


If you have signed my old key(s), I would appreciate signatures on my new
key(s) where relevant/possible.

If you have already validated my old key, you can then validate that
the new key is signed by my old key:

  gpg --check-sigs

If you have any questions about this document or this transition, please
contact me via e-mail at &lt;jcamfield@internews.org&gt; or
&lt;jon@openinternetproject.org&gt; and/or &lt;jon@joncamfield.com&gt; or via Signal
(67276 82126 94566 68124 05822 25963 67276 82126 94566 68124 05822 25963).

In solidarity,
Jon Camfield
jcamfield@internews.org / jon@openinternetproject.org
jon@joncamfield.com


-----BEGIN PGP SIGNATURE-----
Version: GnuPG v1

iQIcBAEBCAAGBQJYJgEIAAoJEKmYlZ/5Jr+L/nIP/1/yl4YeHmoWW/tXy1klX5rA
HpP+/dB/9zAjJzfYAtNJqYRjIxlBSnJLkCYn0wmTRsewO/GxsAyLGm0TKyohreb8
tPq2ur8qMNVvhQeKZuZJb3utdDTCMntR8HTGAnn09JFZ2yD5IZtLMmrFS5kL564B
4EQH6rLfyqTc4e9BVDvIB8r1A511BaimQKMCQK5eqH2slNyzF9jzJ/HtSe7XDlP0
cEOJWPHxq9+pODhDU67vD9GWo3fv8bwjnDsU2WZV6vrCTCTOeA7kpL6w6a9dNntD
JhNP9eRTVlD/thE0n/BALsf/2oUmPTTsc2XhqUsChopIbAPn8OCLdie6KC+5KJMD
4zLioRHTNz2uKAEXdAlNJVV5hDadp154iUZU5U3ercXCi2KarN3HYJwI+baAcBVy
M9bgFCF5zLppTZDO6yGIQnsr2TgY//YH4nvKxTa5jxz+adZ9Y1qMiQ8rD5Ue3zre
BIf/DRZCaKzYkSyk+4bVu6s1chLnFtx5rcHgUDpMuTSh2lyilXARUJDXhVProEKG
//4HlhJslsYQvfjTw4MyqWmg6xunFiH1gQxv2lL4jpdM+fuNA01O264e45xE6bjp
04KDwH0T/edOvqtc7v+toVmGbf/YTcrfuJG1Z89A7t7mdQ/NphTY1fjgLgOL+eTD
Qd7UUeDvdPyYJ5ghtijRiQIcBAEBCAAGBQJYJgEIAAoJELRqAcMnDBfx/nIP/iBq
VqYW9JcFjieXO3fUUjr7YjhVK5i2QsTtVtxtAR71bIQK9HLMVsa6C4/Blrk+Tmcn
u+GlJjTSBGAzXi7mp9Gmwfx8IdNJlh/VxVNi2KXlIN5wjPmb1W9uBkM/4wylnlkI
4rBnZnT/uV0xx7gb9O33E1ULGifxv216Vz1bUtrcwSnwW+S1g8g/svy90KbUlVks
H3K394jJ1A0XghNv33E+I094Zk1JGobcMSmKaDmLg5ltv05RspdHJFPUqXkEqcFM
TcQtmSKi7MO1UM5dZ24MQO+/rF+w4H/9Dn3mYbZf6sFkY6HiudCHNf+6/4Grzib7
asWYGoD7+x6NuFcS2IvYFGS2sTp1P+MZTH8a9PFTFksMQwJiEzVLbihV6lcnjPiU
tuDSqZuceAlZERdPvKeo6HQHsohSJoDjSTlkf20apzb0ypDPqDnVoIsNZWNzVA8i
wgwqhW4+CU02H070rdZnA6FQvAeUTjvZhf2V59+epcN5hwByR/hCWBMAmaRjhfXL
VXiQpa1FNgZMIycEC2seiIOGW1kQGdDpMddNPadg8FVqaQrfAD4npPKG82V5NFq3
LvFIRQpD3mPa5hfe2+DkA8pgboAArjO4781DCvWrUrhmGPtp8pRxXFZu1lzaklsf
O5NhaS+W+9gYcWFWys8XK5TIgO/bN4ioogl1EI+4
=0Tfo
-----END PGP SIGNATURE-----


-----BEGIN PGP SIGNATURE-----
Version: GnuPG v1

iEYEAREIAAYFAlgmATYACgkQKCQ5HrENBEBu3ACgot9j73mzJcYQie5/w2bwX/Hu
cXYAnjVuEJNmjHNzyN4jcyn3248RjpMDiQIcBAEBCAAGBQJYJgE2AAoJELRqAcMn
DBfx3R4P/0rBm6EH5RtH9Tpmv7ac/dCOq5nl53P7V1+auj5BHzcAumwPdiKmOblp
yl3o65XfjoXdSpLoPbzPWdDz5poti3Z3rpscqmKlB3JQ6k4DnPQxFCOtZDW3LCDN
Ll4kCgXEI93G2aY47gJmECzptdUaKOEvYczcsGP1tadJmICdM+mQyJoDfvffn7Gd
k6ImBWJXDazi3Z6zo0u6IUcqk31IEsX33WcrU8myXI6Ks/udLsoAyzwcMnJuvaMl
ZY17FDnCCibCETgA937Mb0y337l6uE1bpHjh15AKLsKl18RMK/x0om5ulTaGrLxm
1/5vGakX6nK6g8bw4fNgXy7BQ0ep/+RlR2FbSKfaNqMkizYTAl9lann6OI69NPKQ
MARX2tqimxK2tzbrWB3NMk39dE7gl5tUoWglEw8rvQH0e0zc/jzmTIY2IjyY5ROc
6PHh6Stk4E8p1qTNIFsYuVkZVx9YZsl1igXkZSpdPKcq7coXNajsyEjCwBDuQT94
z6LsK2lXms+2cvXYKiTt1w4BfJCq12N96Q/L20L17y40j5tkA5sqSSDfUBHiFLCz
2DagmrB7rsILWPFjIzNe0PALbCRcBxxW1PNy+2nfZ2lNtlkYup+F4RplxzJfTr1Z
GBircu8i/HMD2CxiDqguni1UOv2uXd4g2/pNvlTe1cQhqGPGE9XS
=S9re
-----END PGP SIGNATURE-----
</pre>
