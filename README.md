# hyperbible
_The new revised international KJV-ASV-DRB-DBT-ERV-WBT-WEB-YET-AKJV-WNT version of_ Ecclesiastes.

Each sentence in this translation of _Ecclesiastes_ is drawn uniformly at random from one of ten translations of the Bible on every refresh. Study the text. Learn it. Love it. Live it. Refresh the page and you'll never see it again.

Put slightly differently: this book is sampled from the distributions of possible understandings of _Ecclesiastes_, like a more systematic [Septuagint](https://en.wikipedia.org/wiki/Septuagint). You haven't really understood the text until you've studied the nuances of each of its variations.

Made for [National Novel Generation Month 2017](https://github.com/NaNoGenMo/2017), _Ecclesiastes (KJV-ASV-DRB-DBT-ERV-WBT-WEB-YET-AKJV-WNT)_ runs to 10k words per translation, but as it draws its strength by consuming ten (slightly) different translations of the Bible, the hyperobject weighs in at well above the threshold of 50k.

Much thanks to the King James Bible, American Standard Version, Douay-Rheims Bible, Darby Bible Translation, English Revised Version, Webster Bible Translation, World English Bible, Young's Literal Translation, American KJV, and Weymouth New Testament. (Someone on Twitter noted that not only are there many different translations, there are also many different source texts, which is an important complication to keep in mind while reading!)

Different translations are optimized for different qualities, such as "thought-for-thought" or "word-for-word." Here are three comparisons ([1](http://www.mardel.com/bibleTranslationGuide), [2](http://www.mardel.com/bibleTranslationGuide), [3](https://en.wikipedia.org/wiki/List_of_English_Bible_translations)) and a page on the [Douay-Rheims Bible](https://en.wikipedia.org/wiki/Douay%E2%80%93Rheims_Bible).

I'd be curious to see a quantitative study on the qualities of the translations, such as where the mean words lie in an embedding space.

# Instructions

`bible.hs` is a Haskell file that generates the HTML for the page. You'll need to manually copy the Javascript at the top and bottom of the current `bible.html` into the generated `bible.html`, and edit the generated verses again.

`bible.html` contains the js to randomly sample verses from the different translations.

This repository contains the original corpus for the book, `ecc.txt`, as well as `ecc-nl.txt` if you want to just read all the translations at once. Credit for the full corpus—a truly amazing Excel spreadsheet of ten Bibles—goes to the site [hackathon.bible](http://hackathon.bible), specifically to [Biblehub](http://biblehub.net). (_N.B._ There is a parse error in the corpus in _Exodus_.) 

This book is made out of a spirit of respect and love, not sacrilege.
