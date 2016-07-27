# snytax
i hate syntax highlighters
i really do
repo name is not a typo


this is an attempt to create a syntax highlighting theme for atom that i find okay. i will base it on a style guide i created for university math scripts, which aren't at all like code. but i had a few ideas doing that which i want to use.

## general ideas (tbc)
* too many colours are shit and mainly irritate you. don't do that.
  * if the colours are not structuring but destructuring your code, they probably should be adjusted.
  * use such a small number of colours that you actually recognise them individually and they will actually _help_ you at coding. maybe a max of 4 or so. idk.
  * this also means the highlighting will be very personally adjusted to _me_ and how _i_ program and it will develop over time. fork for your own flavour.
* colours should have a more general meaning. like, not just one syntax thing, but maybe a group of things that have familiar associations.
  * this can probably be quite personal as well. i don't even know.
  * example: green means ~~clean.~~ definition. and maybe even assignments.
* if you associate meanings to colours: *use them!* this is a great way to help your mind, as it already has the right associations.

## concrete ideas
i'm doing this highlighting for js, so this is what i'll base my examples on.
i thought of the following 4 groups and colours:
* standard (colour: black or white)
  * this group is the one that has the "standard text" inside it and renders monochrome
  * this means inside it should be the stuff that is most used in our language and "not anything special"
  * BUT: To seperate all the "non-special" things from each other we can use font weight and stuff
  * in my mind this means:
    * names (of variables and constants)
    * language keywords [bold]
    * comments [lighter font weight than standard, italic]
* assignments (colour: green)
  * this group is for "writing stuff into a thing with a name"
  * in my mind this means:
    * assigning a value to a thing with a name. in js this means the = character: `y = 'abc';` has `y` and `''` from the standard group and `=` from assignment group.
    * name definitions: when a name gets defined, like in `const x = 15;`: `const` is a keyword (standard group), `x =` is both in the definition group.
* literals (colour: blue)
  * this group is for "writing a literal value"
  * in my mind this means:
    * numbers
    * strings (but beware: " ", \` \`, / / and so on are language keywords, so they shouldn't be coloured)
    * bools (true/false)
    * object literals (this weird json-y thing in js)
* function calls (colour: red)
  * this group is for the action of calling a function (not just the name of one, a non-invoked name is in the standard group)
  * in my mind this means:
    * names that get invoked. example `awesomeSnytax(value);`. `awesomeSnytax` should be red, parantheses are standard group though.
    * infix operators, like `===` and `||` and `&`, these are also just function calls that take arguments from the left and right side and return something.

## FAQBM
(frequently asked questions by myself)

### when will you start actually making the thing?
idk. maybe tomorrow. or the day after. or next week. maybe not at all, if that's the case just feel inspired and fork this or do your own. i don't care.
### why are you using UK english?
idk. it felt appropriate for somehow ranting about shitty syntax highlighters.
