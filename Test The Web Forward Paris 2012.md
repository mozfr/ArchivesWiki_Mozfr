Quelques conférences sur les tests et les bugs, puis un hackathon pour écrire des tests sur html5, css, indexDB… (et des trucs plus obscures comme [WebIDL](http://www.w3.org/TR/WebIDL/))

Il y avait pas mal de gens du CSSWG (David Baron, Fantasai, Daniel Glazman…) pendant le hackathon, ce qui était sympathique pour poser des questions ou voir leurs échanges pendant qu'ils travaillaient :o)

Mozilliens francophones : Jeremie, David Bruant, Thomas Bassetto, Anthony Ricaud, Pandark

### Premier jour
Quelques confs pour préparer le hackathon du lendemain

#### Welcome Introduction (Vincent Hardy, Adobe)

#### How to Read a Spec (Robin Berjon, W3C)=
http://www.w3.org/TR/

#### How to Create a W3C Reftest (Rebecca Hauck, Adobe)=
http://leaverou.github.com/prefixfree/

#### Overview of testharness.js (James Graham, Opera)=
 /* http://darobin.github.com/test-harness-tutorial/docs/using-testharness.html 
 https://github.com/jgraham/testharness.js */
 &lt;script src=&quot;/ressources/testharness.js&quot;&gt;
 &lt;script src=&quot;/ressources/testharnessreport.js&quot;&gt;
Test are isolated even if they are in the same file

#### File the Best Bug (fantasai, Mozilla)=
Not too short description/name
Don’t link to your website, attach your tests
If needed video (very interactive bug…), use screencast.com

#### Lightning Talks / Meet the Experts

##### Apache Cordova (chromeless browser with w3c draft implemented)
Mobile, phonegap, …

##### Test indexDB (opera)
Use Editor’s Draft, not TR, red not blue :oÞ
ie10, opera, webkit, fx (v.16 new API)

The ordering of exceptions is not defined in the spec yet
→ check common order in browser and add to the spec…
 /*
 localStorage = syncrone
 inndexDB = async, bigger…
 */

##### See if there are test for a section of the spec (ms)

##### w3c html5 testing task force (ms)
→ http://www.w3c-test.org/html/tests/reporting/TestTheWebForward_Paris_2012.pdf
http://www.w3.org/html/wg/ → Working group
http://www.w3c-test.org/
http://dvcs.w3.org/hg

* http://www.w3.org/html/wg/wiki/Testing *

http://www.w3.org/TR/html5/single-page.html#semantics

##### WebRTC (google)
Prez' + Démo

##### CSS3 values (ulb ?)
http://www.w3.org/TR/css3-values/
not very tested, bugs in many implementations
attribut reference
not very much implemented

##### CSS transform (adobe ?)


##### Mingle / Plan for Saturday Hacking

### Deuxième jour
Hackathon : écriture de tests sur HTML5, CSS et autres WebIDL, ou portages de tests d'Apache Cordova (utilisant jasmine.js) vers des tests utilisables par le w3c (utilisant testharness.js)