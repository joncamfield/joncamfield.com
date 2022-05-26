---
excerpt: "A review of a review, and a lot of discussion of password security, chaos, and entropy."
categories:
- hactivismo
- human rights
- crypto
tags:
- information theory
- shannon
- passwords

header:
  overlay_image: /assets/images/pietro-jeng-266017.resized.png
  teaser: /assets/images/pietro-jeng-266017.resized.png
  caption: "Photo CC0 Pietro Jeng / Unsplash"


title: 'Entropy Story-time: From Claude Shannon to Equifax'
created: 1505084712
---
There's an piece floating around that does a great, succinct job at summarizing Claude Shannon's contributions to our modern understanding of information.  If you haven't read <a href="https://aeon.co/essays/how-a-polymath-transformed-our-understanding-of-information">The bit bomb</a> on Aeon, head over there.  It'll make your brain happy with things like this:

<blockquote>"Shannon – mathematician, American, jazz fanatic, juggling enthusiast – is the founder of information theory, and the architect of our digital world. It was Shannon’s paper ‘A Mathematical Theory of Communication’ (1948) that introduced the bit, an objective measure of how much information a message contains."</blockquote>

The article digs deep into how easy it is to predict things - especially language.  It ends up focusing on the power of pattern detection in being able to compress information:

<blockquote>"Shannon expanded this point by turning to a pulpy Raymond Chandler detective story […] He flipped to a random passage … then read out letter by letter to his wife, Betty. Her role was to guess each subsequent letter […] Betty’s job grew progressively easier as context accumulated […] a phrase beginning ‘a small oblong reading lamp on the’ is very likely to be followed by one of two letters: D, or Betty’s first guess, T (presumably for ‘table’). In a zero-redundancy language using our alphabet, Betty would have had only a 1-in-26 chance of guessing correctly; in our language, by contrast, her odds were closer to 1-in-2. " </blockquote>

<h3>Humans Vs. Randomness</h3>
Written English, overall, is up to 75 percent redundant (try this for yourself! Download a huge book in plaint text from <a href="https://www.gutenberg.org/">Project Gutenberg</a> and zip it up to see compression in action).

The amount that this is <strong>difficult</strong> to guess is called entropy, and Shannon's work on this is central to cryptography and secure passwords. You can actually calculate the (maximum) entropy of a collection of letters using his work -- these wikipedia articles are good explainers: <a href="https://en.wikipedia.org/wiki/Password_strength#Entropy_as_a_measure_of_password_strength">Entropy and Password Strength</a> and <a href="https://en.wikipedia.org/wiki/Entropy_(information_theory)">Information Theory and Entropy</a>.

<a href="https://www.datagenetics.com/blog/september32012/"><img src="https://i.guim.co.uk/img/static/sys-images/Money/Pix/pictures/2012/9/28/1348826974847/Top-20-pin-numbers-001.jpg?w=620&q=55&auto=format&usm=12&fit=max&s=803d25db0e135df1f6fe0fda9aa05b9f" align="right" alt="datagenetics" /></a>DataGenetics put out a post on the <a href="https://www.datagenetics.com/blog/september32012/">entropy in your average PIN number</a>. Their table is particularly fun to think through - a totally random number (0-9) has 3.3 "bits" of entropy (specifically, it would take 10 guesses (2^3.3) to guarantee you guess the right number.  You can simply add the entropy bit calculation when adding more numbers, so your average 4-digit PIN is 3.3+3.3+3.3+3.3 or 13.2, or 2^13.2 guesses (9410).

<h3>A short aside on "key length"</h3>
As a rough comparison, "128 bit" encryption is referring to this same number, so to guarantee you will correctly guess the right decryption key takes 2^128 guesses, which is 3.402823669×10³⁸ , which is... a lot of guesses.

It's worth noting that this number only tracks "symmetric" encryption - things like the <a href="https://en.wikipedia.org/wiki/Advanced_Encryption_Standard">Advanced Encryption Standard</a>, more commonly known as AES. Symmetric encryption uses the same key for encrypting and decrypting the data.

You might be more familiar on a daily basis with asymmetric encryption, which is the key (hah) to how the everything from the green lock showing secure websites to <a href="https://www.joncamfield.com/blog/2017.01/lets-talk-about-pgp">super-secure PGP based emails work</a>.  Asymmetric encryption is tracked on a different scale (most asymmetric crypto systems use the public/private system to create a secure symmetric system underneath).  So your 2048 bit PGP key is strong, but actually closer to 128 bits of entropy, because … well, this <a href="https://crypto.stackexchange.com/questions/6236/why-does-the-recommended-key-size-between-symmetric-and-asymmetric-encryption-di">StackExchange discussion</a> is a somewhat readable explanation.

<h3>A quick history lesson</h3>
Nevertheless, you can see why that bit length is very important in terms of how hard it is to guess.  The precursor to AES, DES ("Data Encryption Standard" -- thankfully the creativity on the formal names does not impact their security), was 56 bits.  EFF demonstrated that generally available computational power in the late 90s could <a href="https://en.wikipedia.org/wiki/EFF_DES_cracker">crack DES in a reasonable timeframe</a>.

Bonus fun story - the <a href="https://en.wikipedia.org/wiki/Advanced_Encryption_Standard_process">process to select the algorithm behind AES</a> is a worthwhile read, especially in the context of the ongoing <a href="https://en.wikipedia.org/wiki/Crypto_Wars">Crypto Wars</a> at the time, and the classification of cryptography as an export-controlled munition.

Oh, the 90s.

<h3>Computers (and Countries) Vs. Randomness</h3>
Despite our apparent love of chaos, humans are *horrible* and randomness, and Shannon's information theory work around predictable patterns really shreds this wonderful difficulty of guessing things. As an(other) aside, computers are also not great at randomness, so there's a lot of work to make good "pseudo random" number generators in software, which draw on the timings of keyboard presses, temperature, and mouse movement to "seed" their randomness. Some really interesting reading can be found on Wikipedia on <a href="https://en.wikipedia.org/wiki/Random_number_generation#.22True.22_vs._pseudo-random_numbers">Randon Number Generators</a>, including <a href="https://en.wikipedia.org/wiki/RdRand">international intrigue</a> and <a href="https://en.wikipedia.org/wiki//dev/random">even geekier discussions.</a>

Somewhere between the international intrigue (remember that time the <a href="https://www.nytimes.com/interactive/2013/09/05/us/documents-reveal-nsa-campaign-against-encryption.html">NSA backdoored hardware random number generators</a>?) and a desire to maintain a domestic ability to do the same by blocking powerful random number generators is the why many countries have policies blocking the import of advanced encryption and even laptops with specific hardware random number generators -- for example, China, Russia, Belarus, and Kazakhstan all block computers with TPM chips.

<h3>I thought this was going to be about the data breach?</h3>
I know. You came here for the click bait on Equifax. Stick with me, I'm trying to make this a teachable moment here.

First -- back to PINs. Humans just don't select random numbers, we select patterns like 1234, 1111, 2222, or 2580 (a line straight down the keypad).  You have a 1 in 5 chance of guessing a PIN by trying just five common ones: 1234 (10%), 1111 (6%), 0000 (2%), 1212 (1%), and 7777 (1%).  With 426 guesses from the most common PINs list, you've crossed the 50% mark.

Beyond that, you can still have some wins by limiting your guesses to specific patterns (for example, limiting your guessing to numbers that would fit a MMYY pattern to find birthdays or anniversaries that occurred in, say, the last century) - can vastly improve how well you're able to guess, even if you just know rough the target's rough age.

And don't think that passwords are any better.  Even when not constrained to 4 digits, humans use predictible passwords and the same stupid pattern tricks. There is an annual release of the <a href="https://www.teamsid.com/worst-passwords-2016/?nabe=5285852066611200:1">worst passwords of the year</a> based on whatever big breach leaked passwords. 123456 and password fight for the top spot, and 25 guesses off of top password lists will score you 1 in 10 passwords.

While that number is lower than for PINs, the pattern game in passwords is super fun (add ! at the end, change E to 3!) -- these are easy to program in to a guessing game for a computer. Indeed, people who study passwords create specific rulesets around these specific patterns -- check out <a href="https://contest-2010.korelogic.com/rules.html">these rulesets</a> based on real-world passwords, including automating substituing letters with numbers, swapping out shift-characters (so 1999 would become "!((((" ) and adding dates basically everywhere.

Basically, I have now successfully over-explained the classic <a href="https://xkcd.com/936/">"correct horse battery stable" XKCD comic strip</a>, and we can get on to social security numbers.

<a href="https://xkcd.com/936/"><img src="https://imgs.xkcd.com/comics/password_strength.png" border="0" align="center" alt="XKCD" /></a>

So, <a href="https://www.nytimes.com/2017/09/07/business/equifax-cyberattack.html">Equifax was hacked</a> and Social Security Numbers of 143 million are potentially exposed.

A SSN is 9 digits, so it would theoretically have 30 bits of entropy if the numbers were completely random (9*3.3 = 29.7).

I have some bad news about how random SSNs are.  It's not new information.  In fact, this fine article from <a href="https://phrack.org/issues/19/4.html">Phrack's June 1988 edition</a> details a lot of the patterns behind SSNs (at least for those of us born before 2011) - The first three numbers track to your state, and the next two have specific patterns and sequences that can be predicted given your age.  According to <a href="https://www.pnas.org/content/106/27/10975.full.pdf">this paper</a>, this drops the entropy of your SSN down to 11 bits in some cases - or a mere 2,048 guesses.  This is exactly why you may have seen some phishing emails that have the first 6 digits of your SSN already guessed (and often  verified using free online services) and seek to trick you into revealing the last four digits -- the only ones with any privacy left to them.  It is an exercise left to the user as to why the last four digits of your SSN also make a horrible PIN number for other services.

All of this is to say: be angry that a company who's core business relied on protecting this information failed to do so.  Be extra cautious about identity scams, especially as that same company is doing <a href="https://motherboard.vice.com/en_us/article/mbb8vv/want-to-know-if-your-ssn-was-included-in-the-equifax-breach-good-luck">a horrible job at trustable incident response so far</a>. Look into putting a freeze on new lines of credit in your name. But also remember that the SSN as a secure, unique identifier protects your privacy about as well as the emperor's new clothing protects his.

<em>Crypto-types: Shoot me an email if I've oversimplified a concept to a point you feel is misleading.</em>

<a style="background-color:black;color:white;text-decoration:none;padding:4px 6px;font-family:-apple-system, BlinkMacSystemFont, &quot;San Francisco&quot;, &quot;Helvetica Neue&quot;, Helvetica, Ubuntu, Roboto, Noto, &quot;Segoe UI&quot;, Arial, sans-serif;font-size:12px;font-weight:bold;line-height:1.2;display:inline-block;border-radius:3px;" href="https://unsplash.com/@pietrozj?utm_medium=referral&amp;utm_campaign=photographer-credit&amp;utm_content=creditBadge" target="_blank" rel="noopener noreferrer" title="Download free do whatever you want high-resolution photos from Pietro Jeng"><span style="display:inline-block;padding:2px 3px;"><svg xmlns="https://www.w3.org/2000/svg" style="height:12px;width:auto;position:relative;vertical-align:middle;top:-1px;fill:white;" viewBox="0 0 32 32"><title></title><path d="M20.8 18.1c0 2.7-2.2 4.8-4.8 4.8s-4.8-2.1-4.8-4.8c0-2.7 2.2-4.8 4.8-4.8 2.7.1 4.8 2.2 4.8 4.8zm11.2-7.4v14.9c0 2.3-1.9 4.3-4.3 4.3h-23.4c-2.4 0-4.3-1.9-4.3-4.3v-15c0-2.3 1.9-4.3 4.3-4.3h3.7l.8-2.3c.4-1.1 1.7-2 2.9-2h8.6c1.2 0 2.5.9 2.9 2l.8 2.4h3.7c2.4 0 4.3 1.9 4.3 4.3zm-8.6 7.5c0-4.1-3.3-7.5-7.5-7.5-4.1 0-7.5 3.4-7.5 7.5s3.3 7.5 7.5 7.5c4.2-.1 7.5-3.4 7.5-7.5z"></path></svg></span><span style="display:inline-block;padding:2px 3px;">Pietro Jeng</span></a>
