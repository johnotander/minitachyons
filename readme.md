# minitachyons 0.1.9

A miniscule, opinionated subset of Tachyons

#### Stats

4591 | 674 | 832
---|---|---
bytes | selectors | declarations

## Installation

#### With [npm](https://npmjs.com)

```
npm install --save-dev minitachyons
```

#### With Git

```
git clone https://github.com/tachyons-css/minitachyons
```

## Usage

#### Using with [PostCSS](https://github.com/postcss/postcss)

Import the css module

```css
@import "minitachyons";
```

Then process the CSS using the [`tachyons-cli`](https://github.com/tachyons-css/tachyons-cli)

```sh
$ npm i -g tachyons-cli
$ tachyons-cli path/to/css-file.css > dist/t.css
```

#### Using the CSS

The built CSS is located in the `css` directory. It contains an unminified and minified version.
You can either cut and paste that css or link to it directly in your html.

```html
<link rel="stylesheet" href="path/to/module/css/minitachyons">
```

#### Development

The source CSS files can be found in the `src` directory.
Running `$ npm start` will process the source CSS and place the built CSS in the `css` directory.

## The CSS

```css
@import "normalize.css";
@import "tachyons-border-box";
.br2 { border-radius: .25rem; }
.normal { font-weight: normal; }
.b { font-weight: bold; }
.tracked { letter-spacing: .16em; }
.mid-gray { color: #555; }
.silver { color: #999; }
.light-silver { color: #aaa; }
.ttu { text-transform: uppercase; }
.measure { max-width: 30em; }
.truncate { white-space: nowrap; overflow: hidden; text-overflow: ellipsis; }
.v-mid { vertical-align: middle; }
/*

  BASE

*/
html, body { height: 100%; }
/*

   TYPE SCALE

*/
/* For Hero Titles */
.f-6, .f-headline { font-size: 6rem; }
.f-5, .f-subheadline { font-size: 5rem; }
/* Type Scale */
.f1 { font-size: 3rem; }
.f2 { font-size: 2.25rem; }
.f3 { font-size: 1.5rem; }
.f4 { font-size: 1.25rem; }
.f5 { font-size: 1rem; }
.f6 { font-size: .875rem; }
/* Media Query Variables */
/*

   FLOATS

   1. Floated elements are automatically rendered as block level elements.
      Setting floats to display inline will fix the double margin bug in
      ie6. You know... just in case.

   2. Don't forget to clearfix your floats with .cf

   Base:
     f = float

   Modifiers:
     l = left
     r = right
     n = none

   Media Query Extensions:
     -ns = not-small
     -m  = medium
     -l  = large

*/
.fl { float: left; display: inline; }
.fr { float: right; display: inline; }
.fn { float: none; }
/*

   BORDER BASE

   Legend

   a = all
   t = top
   r = right
   b = bottom
   l = left

*/
.ba { border-style: solid; border-width: 1px; }
.bt { border-top-style: solid; border-top-width: 1px; }
.br { border-right-style: solid; border-right-width: 1px; }
.bb { border-bottom-style: solid; border-bottom-width: 1px; }
.bl { border-left-style: solid; border-left-width: 1px; }
.bn { border-style: none; border-width: 0; }
/*

   LINKS

*/
.link { text-decoration: none; transition: color .15s ease-in; }
.link:link, .link:visited { transition: color .15s ease-in; }
.link:hover { transition: color .15s ease-in; }
.link:active { transition: color .15s ease-in; }
.link:focus { transition: color .15s ease-in; }
/*

   WIDTHS

   Base:
     w = width

   Modifiers
     1 = 1st step in width scale
     2 = 2nd step in width scale
     3 = 3rd step in width scale
     4 = 4th step in width scale
     5 = 5th step in width scale

     -10  = literal value 10%
     -20  = literal value 20%
     -25  = literal value 25%
     -33  = literal value 33%
     -34  = literal value 34%
     -40  = literal value 40%
     -50  = literal value 50%
     -60  = literal value 60%
     -75  = literal value 75%
     -80  = literal value 80%
     -100 = literal value 100%

     -auto  = string value auto


   Media Query Extensions:
     -ns = not-small
     -m  = medium
     -l  = large

*/
/* Width Scale */
.w1 { width: 1rem; }
.w2 { width: 2rem; }
.w3 { width: 4rem; }
.w4 { width: 8rem; }
.w5 { width: 16rem; }
.w-10 { width: 10%; }
.w-20 { width: 20%; }
.w-25 { width: 25%; }
.w-33 { width: 33%; }
.w-34 { width: 34%; }
.w-40 { width: 40%; }
.w-50 { width: 50%; }
.w-60 { width: 60%; }
.w-75 { width: 75%; }
.w-80 { width: 80%; }
.w-100 { width: 100%; }
.w-auto { width: auto; }
/* Variables */
/* Spacing Scale - based on a ratio of 1:2 */
/* Media Queries */
/*
   SPACING

   An eight step powers of two scale ranging from 0 to 16rem.
   Namespaces are composable and thus highly grockable - check the legend below

   Legend:

   p = padding
   m = margin

   a = all
   h = horizontal
   v = vertical
   t = top
   r = right
   b = bottom
   l = left

   0 = none
   1 = 1st step in spacing scale
   2 = 2nd step in spacing scale
   3 = 3rd step in spacing scale
   4 = 4th step in spacing scale
   5 = 5th step in spacing scale
   6 = 6th step in spacing scale
   7 = 7th step in spacing scale

*/
.pa0 { padding: 0; }
.pa1 { padding: .25rem; }
.pa2 { padding: .5rem; }
.pa3 { padding: 1rem; }
.pa4 { padding: 2rem; }
.pa5 { padding: 4rem; }
.pa6 { padding: 8rem; }
.pa7 { padding: 16rem; }
.pl0 { padding-left: 0; }
.pl1 { padding-left: .25rem; }
.pl2 { padding-left: .5rem; }
.pl3 { padding-left: 1rem; }
.pl4 { padding-left: 2rem; }
.pl5 { padding-left: 4rem; }
.pl6 { padding-left: 8rem; }
.pl7 { padding-left: 16rem; }
.pr0 { padding-right: 0; }
.pr1 { padding-right: .25rem; }
.pr2 { padding-right: .5rem; }
.pr3 { padding-right: 1rem; }
.pr4 { padding-right: 2rem; }
.pr5 { padding-right: 4rem; }
.pr6 { padding-right: 8rem; }
.pr7 { padding-right: 16rem; }
.pb0 { padding-bottom: 0; }
.pb1 { padding-bottom: .25rem; }
.pb2 { padding-bottom: .5rem; }
.pb3 { padding-bottom: 1rem; }
.pb4 { padding-bottom: 2rem; }
.pb5 { padding-bottom: 4rem; }
.pb6 { padding-bottom: 8rem; }
.pb7 { padding-bottom: 16rem; }
.pt0 { padding-top: 0; }
.pt1 { padding-top: .25rem; }
.pt2 { padding-top: .5rem; }
.pt3 { padding-top: 1rem; }
.pt4 { padding-top: 2rem; }
.pt5 { padding-top: 4rem; }
.pt6 { padding-top: 8rem; }
.pt7 { padding-top: 16rem; }
.pv0 { padding-top: 0; padding-bottom: 0; }
.pv1 { padding-top: .25rem; padding-bottom: .25rem; }
.pv2 { padding-top: .5rem; padding-bottom: .5rem; }
.pv3 { padding-top: 1rem; padding-bottom: 1rem; }
.pv4 { padding-top: 2rem; padding-bottom: 2rem; }
.pv5 { padding-top: 4rem; padding-bottom: 4rem; }
.pv6 { padding-top: 8rem; padding-bottom: 8rem; }
.pv7 { padding-top: 16rem; padding-bottom: 16rem; }
.ph0 { padding-left: 0; padding-right: 0; }
.ph1 { padding-left: .25rem; padding-right: .25rem; }
.ph2 { padding-left: .5rem; padding-right: .5rem; }
.ph3 { padding-left: 1rem; padding-right: 1rem; }
.ph4 { padding-left: 2rem; padding-right: 2rem; }
.ph5 { padding-left: 4rem; padding-right: 4rem; }
.ph6 { padding-left: 8rem; padding-right: 8rem; }
.ph7 { padding-left: 16rem; padding-right: 16rem; }
.ma0 { margin: 0; }
.ma1 { margin: .25rem; }
.ma2 { margin: .5rem; }
.ma3 { margin: 1rem; }
.ma4 { margin: 2rem; }
.ma5 { margin: 4rem; }
.ma6 { margin: 8rem; }
.ma7 { margin: 16rem; }
.ml0 { margin-left: 0; }
.ml1 { margin-left: .25rem; }
.ml2 { margin-left: .5rem; }
.ml3 { margin-left: 1rem; }
.ml4 { margin-left: 2rem; }
.ml5 { margin-left: 4rem; }
.ml6 { margin-left: 8rem; }
.ml7 { margin-left: 16rem; }
.mr0 { margin-right: 0; }
.mr1 { margin-right: .25rem; }
.mr2 { margin-right: .5rem; }
.mr3 { margin-right: 1rem; }
.mr4 { margin-right: 2rem; }
.mr5 { margin-right: 4rem; }
.mr6 { margin-right: 8rem; }
.mr7 { margin-right: 16rem; }
.mb0 { margin-bottom: 0; }
.mb1 { margin-bottom: .25rem; }
.mb2 { margin-bottom: .5rem; }
.mb3 { margin-bottom: 1rem; }
.mb4 { margin-bottom: 2rem; }
.mb5 { margin-bottom: 4rem; }
.mb6 { margin-bottom: 8rem; }
.mb7 { margin-bottom: 16rem; }
.mt0 { margin-top: 0; }
.mt1 { margin-top: .25rem; }
.mt2 { margin-top: .5rem; }
.mt3 { margin-top: 1rem; }
.mt4 { margin-top: 2rem; }
.mt5 { margin-top: 4rem; }
.mt6 { margin-top: 8rem; }
.mt7 { margin-top: 16rem; }
.mv0 { margin-top: 0; margin-bottom: 0; }
.mv1 { margin-top: .25rem; margin-bottom: .25rem; }
.mv2 { margin-top: .5rem; margin-bottom: .5rem; }
.mv3 { margin-top: 1rem; margin-bottom: 1rem; }
.mv4 { margin-top: 2rem; margin-bottom: 2rem; }
.mv5 { margin-top: 4rem; margin-bottom: 4rem; }
.mv6 { margin-top: 8rem; margin-bottom: 8rem; }
.mv7 { margin-top: 16rem; margin-bottom: 16rem; }
.mh0 { margin-left: 0; margin-right: 0; }
.mh1 { margin-left: .25rem; margin-right: .25rem; }
.mh2 { margin-left: .5rem; margin-right: .5rem; }
.mh3 { margin-left: 1rem; margin-right: 1rem; }
.mh4 { margin-left: 2rem; margin-right: 2rem; }
.mh5 { margin-left: 4rem; margin-right: 4rem; }
.mh6 { margin-left: 8rem; margin-right: 8rem; }
.mh7 { margin-left: 16rem; margin-right: 16rem; }
/*

  TABLES

*/
.collapse { border-collapse: collapse; border-spacing: 0; }
.striped--moon-gray:nth-child(odd) { background-color: #aaa; }
.striped--moon-gray:nth-child(odd) { background-color: #ccc; }
.striped--light-gray:nth-child(odd) { background-color: #eee; }
.striped--near-white:nth-child(odd) { background-color: #f4f4f4; }
/*

   DISPLAY

   Base:
    d = display

   Modifiers:
    n     = none
    b     = block
    ib    = inline-block
    it    = inline-table
    t     = table
    tc    = table-cell
    tr    = table-row
    tcol  = table-column
    tcolg = table-column-group

   Media Query Extensions:
     -ns = not-small
     -m  = medium
     -l  = large

*/
.dn { display: none; }
.di { display: inline; }
.db { display: block; }
.dib { display: inline-block; }
.dit { display: inline-table; }
.dt { display: table; }
.dtc { display: table-cell; }
.dt-row { display: table-row; }
.dt-row-group { display: table-row-group; }
.dt-column { display: table-column; }
.dt-column-group { display: table-column-group; }
/*
  This will set table to full width and then
  all cells will be equal width
*/
.dt--fixed { table-layout: fixed; width: 100%; }
body { font-family: -apple-system, BlinkMacSystemFont, 'avenir next', avenir, helvetica, 'helvetica neue', ubuntu, roboto, noto, 'segoe ui', arial, sans-serif; }
/* Nicolas Gallaghers Clearfix solution
 *    Ref: http://nicolasgallagher.com/micro-clearfix-hack/ */
.cf:before, .cf:after { content: " "; display: table; }
.cf:after { clear: both; }
.cf { *zoom: 1; }
.blg { border-color: #aaa; }
@media screen and (min-width: 30em) {
 .normal-ns { font-weight: normal; }
 .b-ns { font-weight: bold; }
 .measure-ns { max-width: 30em; }
 .v-mid-ns { vertical-align: middle; }
}
@media screen and (min-width: 30em) and (max-width: 60em) { }
@media screen and (min-width: 60em) { }
@media screen and (min-width: 48em) {
 .f-6-ns, .f-headline-ns { font-size: 6rem; }
 .f-5-ns, .f-subheadline-ns { font-size: 5rem; }
 .f1-ns { font-size: 3rem; }
 .f2-ns { font-size: 2.25rem; }
 .f3-ns { font-size: 1.5rem; }
 .f4-ns { font-size: 1.25rem; }
 .f5-ns { font-size: 1rem; }
 .f6-ns { font-size: .875rem; }
 .fl-ns { float: left; display: inline; }
 .fr-ns { float: right; display: inline; }
 .fn-ns { float: none; }
 .ba-ns { border-style: solid; border-width: 1px; }
 .bt-ns { border-top-style: solid; border-top-width: 1px; }
 .br-ns { border-right-style: solid; border-right-width: 1px; }
 .bb-ns { border-bottom-style: solid; border-bottom-width: 1px; }
 .bl-ns { border-left-style: solid; border-left-width: 1px; }
 .bn-ns { border-style: none; border-width: 0; }
 .w1-ns { width: 1rem; }
 .w2-ns { width: 2rem; }
 .w3-ns { width: 4rem; }
 .w4-ns { width: 8rem; }
 .w5-ns { width: 16rem; }
 .w-10-ns { width: 10%; }
 .w-20-ns { width: 20%; }
 .w-25-ns { width: 25%; }
 .w-33-ns { width: 33%; }
 .w-34-ns { width: 34%; }
 .w-40-ns { width: 40%; }
 .w-50-ns { width: 50%; }
 .w-60-ns { width: 60%; }
 .w-75-ns { width: 75%; }
 .w-80-ns { width: 80%; }
 .w-100-ns { width: 100%; }
 .w-auto-ns { width: auto; }
 .pa0-ns { padding: 0; }
 .pa1-ns { padding: .25rem; }
 .pa2-ns { padding: .5rem; }
 .pa3-ns { padding: 1rem; }
 .pa4-ns { padding: 2rem; }
 .pa5-ns { padding: 4rem; }
 .pa6-ns { padding: 8rem; }
 .pa7-ns { padding: 16rem; }
 .pl0-ns { padding-left: 0; }
 .pl1-ns { padding-left: .25rem; }
 .pl2-ns { padding-left: .5rem; }
 .pl3-ns { padding-left: 1rem; }
 .pl4-ns { padding-left: 2rem; }
 .pl5-ns { padding-left: 4rem; }
 .pl6-ns { padding-left: 8rem; }
 .pl7-ns { padding-left: 16rem; }
 .pr0-ns { padding-right: 0; }
 .pr1-ns { padding-right: .25rem; }
 .pr2-ns { padding-right: .5rem; }
 .pr3-ns { padding-right: 1rem; }
 .pr4-ns { padding-right: 2rem; }
 .pr5-ns { padding-right: 4rem; }
 .pr6-ns { padding-right: 8rem; }
 .pr7-ns { padding-right: 16rem; }
 .pb0-ns { padding-bottom: 0; }
 .pb1-ns { padding-bottom: .25rem; }
 .pb2-ns { padding-bottom: .5rem; }
 .pb3-ns { padding-bottom: 1rem; }
 .pb4-ns { padding-bottom: 2rem; }
 .pb5-ns { padding-bottom: 4rem; }
 .pb6-ns { padding-bottom: 8rem; }
 .pb7-ns { padding-bottom: 16rem; }
 .pt0-ns { padding-top: 0; }
 .pt1-ns { padding-top: .25rem; }
 .pt2-ns { padding-top: .5rem; }
 .pt3-ns { padding-top: 1rem; }
 .pt4-ns { padding-top: 2rem; }
 .pt5-ns { padding-top: 4rem; }
 .pt6-ns { padding-top: 8rem; }
 .pt7-ns { padding-top: 16rem; }
 .pv0-ns { padding-top: 0; padding-bottom: 0; }
 .pv1-ns { padding-top: .25rem; padding-bottom: .25rem; }
 .pv2-ns { padding-top: .5rem; padding-bottom: .5rem; }
 .pv3-ns { padding-top: 1rem; padding-bottom: 1rem; }
 .pv4-ns { padding-top: 2rem; padding-bottom: 2rem; }
 .pv5-ns { padding-top: 4rem; padding-bottom: 4rem; }
 .pv6-ns { padding-top: 8rem; padding-bottom: 8rem; }
 .pv7-ns { padding-top: 16rem; padding-bottom: 16rem; }
 .ph0-ns { padding-left: 0; padding-right: 0; }
 .ph1-ns { padding-left: .25rem; padding-right: .25rem; }
 .ph2-ns { padding-left: .5rem; padding-right: .5rem; }
 .ph3-ns { padding-left: 1rem; padding-right: 1rem; }
 .ph4-ns { padding-left: 2rem; padding-right: 2rem; }
 .ph5-ns { padding-left: 4rem; padding-right: 4rem; }
 .ph6-ns { padding-left: 8rem; padding-right: 8rem; }
 .ph7-ns { padding-left: 16rem; padding-right: 16rem; }
 .ma0-ns { margin: 0; }
 .ma1-ns { margin: .25rem; }
 .ma2-ns { margin: .5rem; }
 .ma3-ns { margin: 1rem; }
 .ma4-ns { margin: 2rem; }
 .ma5-ns { margin: 4rem; }
 .ma6-ns { margin: 8rem; }
 .ma7-ns { margin: 16rem; }
 .ml0-ns { margin-left: 0; }
 .ml1-ns { margin-left: .25rem; }
 .ml2-ns { margin-left: .5rem; }
 .ml3-ns { margin-left: 1rem; }
 .ml4-ns { margin-left: 2rem; }
 .ml5-ns { margin-left: 4rem; }
 .ml6-ns { margin-left: 8rem; }
 .ml7-ns { margin-left: 16rem; }
 .mr0-ns { margin-right: 0; }
 .mr1-ns { margin-right: .25rem; }
 .mr2-ns { margin-right: .5rem; }
 .mr3-ns { margin-right: 1rem; }
 .mr4-ns { margin-right: 2rem; }
 .mr5-ns { margin-right: 4rem; }
 .mr6-ns { margin-right: 8rem; }
 .mr7-ns { margin-right: 16rem; }
 .mb0-ns { margin-bottom: 0; }
 .mb1-ns { margin-bottom: .25rem; }
 .mb2-ns { margin-bottom: .5rem; }
 .mb3-ns { margin-bottom: 1rem; }
 .mb4-ns { margin-bottom: 2rem; }
 .mb5-ns { margin-bottom: 4rem; }
 .mb6-ns { margin-bottom: 8rem; }
 .mb7-ns { margin-bottom: 16rem; }
 .mt0-ns { margin-top: 0; }
 .mt1-ns { margin-top: .25rem; }
 .mt2-ns { margin-top: .5rem; }
 .mt3-ns { margin-top: 1rem; }
 .mt4-ns { margin-top: 2rem; }
 .mt5-ns { margin-top: 4rem; }
 .mt6-ns { margin-top: 8rem; }
 .mt7-ns { margin-top: 16rem; }
 .mv0-ns { margin-top: 0; margin-bottom: 0; }
 .mv1-ns { margin-top: .25rem; margin-bottom: .25rem; }
 .mv2-ns { margin-top: .5rem; margin-bottom: .5rem; }
 .mv3-ns { margin-top: 1rem; margin-bottom: 1rem; }
 .mv4-ns { margin-top: 2rem; margin-bottom: 2rem; }
 .mv5-ns { margin-top: 4rem; margin-bottom: 4rem; }
 .mv6-ns { margin-top: 8rem; margin-bottom: 8rem; }
 .mv7-ns { margin-top: 16rem; margin-bottom: 16rem; }
 .mh0-ns { margin-left: 0; margin-right: 0; }
 .mh1-ns { margin-left: .25rem; margin-right: .25rem; }
 .mh2-ns { margin-left: .5rem; margin-right: .5rem; }
 .mh3-ns { margin-left: 1rem; margin-right: 1rem; }
 .mh4-ns { margin-left: 2rem; margin-right: 2rem; }
 .mh5-ns { margin-left: 4rem; margin-right: 4rem; }
 .mh6-ns { margin-left: 8rem; margin-right: 8rem; }
 .mh7-ns { margin-left: 16rem; margin-right: 16rem; }
 .dn-ns { display: none; }
 .di-ns { display: inline; }
 .db-ns { display: block; }
 .dib-ns { display: inline-block; }
 .dit-ns { display: inline-table; }
 .dt-ns { display: table; }
 .dtc-ns { display: table-cell; }
 .dt-row-ns { display: table-row; }
 .dt-row-group-ns { display: table-row-group; }
 .dt-column-ns { display: table-column; }
 .dt-column-group-ns { display: table-column-group; }
 .dt--fixed-ns { table-layout: fixed; width: 100%; }
}
@media screen and (min-width: 48em) and (max-width: 64em) {
 .f-6-m, .f-headline-m { font-size: 6rem; }
 .f-5-m, .f-subheadline-m { font-size: 5rem; }
 .f1-m { font-size: 3rem; }
 .f2-m { font-size: 2.25rem; }
 .f3-m { font-size: 1.5rem; }
 .f4-m { font-size: 1.25rem; }
 .f5-m { font-size: 1rem; }
 .f6-m { font-size: .875rem; }
 .fl-m { float: left; display: inline; }
 .fr-m { float: right; display: inline; }
 .fn-m { float: none; }
 .ba-m { border-style: solid; border-width: 1px; }
 .bt-m { border-top-style: solid; border-top-width: 1px; }
 .br-m { border-right-style: solid; border-right-width: 1px; }
 .bb-m { border-bottom-style: solid; border-bottom-width: 1px; }
 .bl-m { border-left-style: solid; border-left-width: 1px; }
 .bn-m { border-style: none; border-width: 0; }
 .w1-m { width: 1rem; }
 .w2-m { width: 2rem; }
 .w3-m { width: 4rem; }
 .w4-m { width: 8rem; }
 .w5-m { width: 16rem; }
 .w-10-m { width: 10%; }
 .w-20-m { width: 20%; }
 .w-25-m { width: 25%; }
 .w-33-m { width: 33%; }
 .w-34-m { width: 34%; }
 .w-40-m { width: 40%; }
 .w-50-m { width: 50%; }
 .w-60-m { width: 60%; }
 .w-75-m { width: 75%; }
 .w-80-m { width: 80%; }
 .w-100-m { width: 100%; }
 .w-auto-m { width: auto; }
 .pa0-m { padding: 0; }
 .pa1-m { padding: .25rem; }
 .pa2-m { padding: .5rem; }
 .pa3-m { padding: 1rem; }
 .pa4-m { padding: 2rem; }
 .pa5-m { padding: 4rem; }
 .pa6-m { padding: 8rem; }
 .pa7-m { padding: 16rem; }
 .pl0-m { padding-left: 0; }
 .pl1-m { padding-left: .25rem; }
 .pl2-m { padding-left: .5rem; }
 .pl3-m { padding-left: 1rem; }
 .pl4-m { padding-left: 2rem; }
 .pl5-m { padding-left: 4rem; }
 .pl6-m { padding-left: 8rem; }
 .pl7-m { padding-left: 16rem; }
 .pr0-m { padding-right: 0; }
 .pr1-m { padding-right: .25rem; }
 .pr2-m { padding-right: .5rem; }
 .pr3-m { padding-right: 1rem; }
 .pr4-m { padding-right: 2rem; }
 .pr5-m { padding-right: 4rem; }
 .pr6-m { padding-right: 8rem; }
 .pr7-m { padding-right: 16rem; }
 .pb0-m { padding-bottom: 0; }
 .pb1-m { padding-bottom: .25rem; }
 .pb2-m { padding-bottom: .5rem; }
 .pb3-m { padding-bottom: 1rem; }
 .pb4-m { padding-bottom: 2rem; }
 .pb5-m { padding-bottom: 4rem; }
 .pb6-m { padding-bottom: 8rem; }
 .pb7-m { padding-bottom: 16rem; }
 .pt0-m { padding-top: 0; }
 .pt1-m { padding-top: .25rem; }
 .pt2-m { padding-top: .5rem; }
 .pt3-m { padding-top: 1rem; }
 .pt4-m { padding-top: 2rem; }
 .pt5-m { padding-top: 4rem; }
 .pt6-m { padding-top: 8rem; }
 .pt7-m { padding-top: 16rem; }
 .pv0-m { padding-top: 0; padding-bottom: 0; }
 .pv1-m { padding-top: .25rem; padding-bottom: .25rem; }
 .pv2-m { padding-top: .5rem; padding-bottom: .5rem; }
 .pv3-m { padding-top: 1rem; padding-bottom: 1rem; }
 .pv4-m { padding-top: 2rem; padding-bottom: 2rem; }
 .pv5-m { padding-top: 4rem; padding-bottom: 4rem; }
 .pv6-m { padding-top: 8rem; padding-bottom: 8rem; }
 .pv7-m { padding-top: 16rem; padding-bottom: 16rem; }
 .ph0-m { padding-left: 0; padding-right: 0; }
 .ph1-m { padding-left: .25rem; padding-right: .25rem; }
 .ph2-m { padding-left: .5rem; padding-right: .5rem; }
 .ph3-m { padding-left: 1rem; padding-right: 1rem; }
 .ph4-m { padding-left: 2rem; padding-right: 2rem; }
 .ph5-m { padding-left: 4rem; padding-right: 4rem; }
 .ph6-m { padding-left: 8rem; padding-right: 8rem; }
 .ph7-m { padding-left: 16rem; padding-right: 16rem; }
 .ma0-m { margin: 0; }
 .ma1-m { margin: .25rem; }
 .ma2-m { margin: .5rem; }
 .ma3-m { margin: 1rem; }
 .ma4-m { margin: 2rem; }
 .ma5-m { margin: 4rem; }
 .ma6-m { margin: 8rem; }
 .ma7-m { margin: 16rem; }
 .ml0-m { margin-left: 0; }
 .ml1-m { margin-left: .25rem; }
 .ml2-m { margin-left: .5rem; }
 .ml3-m { margin-left: 1rem; }
 .ml4-m { margin-left: 2rem; }
 .ml5-m { margin-left: 4rem; }
 .ml6-m { margin-left: 8rem; }
 .ml7-m { margin-left: 16rem; }
 .mr0-m { margin-right: 0; }
 .mr1-m { margin-right: .25rem; }
 .mr2-m { margin-right: .5rem; }
 .mr3-m { margin-right: 1rem; }
 .mr4-m { margin-right: 2rem; }
 .mr5-m { margin-right: 4rem; }
 .mr6-m { margin-right: 8rem; }
 .mr7-m { margin-right: 16rem; }
 .mb0-m { margin-bottom: 0; }
 .mb1-m { margin-bottom: .25rem; }
 .mb2-m { margin-bottom: .5rem; }
 .mb3-m { margin-bottom: 1rem; }
 .mb4-m { margin-bottom: 2rem; }
 .mb5-m { margin-bottom: 4rem; }
 .mb6-m { margin-bottom: 8rem; }
 .mb7-m { margin-bottom: 16rem; }
 .mt0-m { margin-top: 0; }
 .mt1-m { margin-top: .25rem; }
 .mt2-m { margin-top: .5rem; }
 .mt3-m { margin-top: 1rem; }
 .mt4-m { margin-top: 2rem; }
 .mt5-m { margin-top: 4rem; }
 .mt6-m { margin-top: 8rem; }
 .mt7-m { margin-top: 16rem; }
 .mv0-m { margin-top: 0; margin-bottom: 0; }
 .mv1-m { margin-top: .25rem; margin-bottom: .25rem; }
 .mv2-m { margin-top: .5rem; margin-bottom: .5rem; }
 .mv3-m { margin-top: 1rem; margin-bottom: 1rem; }
 .mv4-m { margin-top: 2rem; margin-bottom: 2rem; }
 .mv5-m { margin-top: 4rem; margin-bottom: 4rem; }
 .mv6-m { margin-top: 8rem; margin-bottom: 8rem; }
 .mv7-m { margin-top: 16rem; margin-bottom: 16rem; }
 .mh0-m { margin-left: 0; margin-right: 0; }
 .mh1-m { margin-left: .25rem; margin-right: .25rem; }
 .mh2-m { margin-left: .5rem; margin-right: .5rem; }
 .mh3-m { margin-left: 1rem; margin-right: 1rem; }
 .mh4-m { margin-left: 2rem; margin-right: 2rem; }
 .mh5-m { margin-left: 4rem; margin-right: 4rem; }
 .mh6-m { margin-left: 8rem; margin-right: 8rem; }
 .mh7-m { margin-left: 16rem; margin-right: 16rem; }
 .dn-m { display: none; }
 .di-m { display: inline; }
 .db-m { display: block; }
 .dib-m { display: inline-block; }
 .dit-m { display: inline-table; }
 .dt-m { display: table; }
 .dtc-m { display: table-cell; }
 .dt-row-m { display: table-row; }
 .dt-row-group-m { display: table-row-group; }
 .dt-column-m { display: table-column; }
 .dt-column-group-m { display: table-column-group; }
 .dt--fixed-m { table-layout: fixed; width: 100%; }
}
@media screen and (min-width: 64em) {
 .f-6-l, .f-headline-l { font-size: 6rem; }
 .f-5-l, .f-subheadline-l { font-size: 5rem; }
 .f1-l { font-size: 3rem; }
 .f2-l { font-size: 2.25rem; }
 .f3-l { font-size: 1.5rem; }
 .f4-l { font-size: 1.25rem; }
 .f5-l { font-size: 1rem; }
 .f6-l { font-size: .875rem; }
 .fl-l { float: left; display: inline; }
 .fr-l { float: right; display: inline; }
 .fn-l { float: none; }
 .ba-l { border-style: solid; border-width: 1px; }
 .bt-l { border-top-style: solid; border-top-width: 1px; }
 .br-l { border-right-style: solid; border-right-width: 1px; }
 .bb-l { border-bottom-style: solid; border-bottom-width: 1px; }
 .bl-l { border-left-style: solid; border-left-width: 1px; }
 .bn-l { border-style: none; border-width: 0; }
 .w1-l { width: 1rem; }
 .w2-l { width: 2rem; }
 .w3-l { width: 4rem; }
 .w4-l { width: 8rem; }
 .w5-l { width: 16rem; }
 .w-10-l { width: 10%; }
 .w-20-l { width: 20%; }
 .w-25-l { width: 25%; }
 .w-33-l { width: 33%; }
 .w-34-l { width: 34%; }
 .w-40-l { width: 40%; }
 .w-50-l { width: 50%; }
 .w-60-l { width: 60%; }
 .w-75-l { width: 75%; }
 .w-80-l { width: 80%; }
 .w-100-l { width: 100%; }
 .w-auto-l { width: auto; }
 .pa0-l { padding: 0; }
 .pa1-l { padding: .25rem; }
 .pa2-l { padding: .5rem; }
 .pa3-l { padding: 1rem; }
 .pa4-l { padding: 2rem; }
 .pa5-l { padding: 4rem; }
 .pa6-l { padding: 8rem; }
 .pa7-l { padding: 16rem; }
 .pl0-l { padding-left: 0; }
 .pl1-l { padding-left: .25rem; }
 .pl2-l { padding-left: .5rem; }
 .pl3-l { padding-left: 1rem; }
 .pl4-l { padding-left: 2rem; }
 .pl5-l { padding-left: 4rem; }
 .pl6-l { padding-left: 8rem; }
 .pl7-l { padding-left: 16rem; }
 .pr0-l { padding-right: 0; }
 .pr1-l { padding-right: .25rem; }
 .pr2-l { padding-right: .5rem; }
 .pr3-l { padding-right: 1rem; }
 .pr4-l { padding-right: 2rem; }
 .pr5-l { padding-right: 4rem; }
 .pr6-l { padding-right: 8rem; }
 .pr7-l { padding-right: 16rem; }
 .pb0-l { padding-bottom: 0; }
 .pb1-l { padding-bottom: .25rem; }
 .pb2-l { padding-bottom: .5rem; }
 .pb3-l { padding-bottom: 1rem; }
 .pb4-l { padding-bottom: 2rem; }
 .pb5-l { padding-bottom: 4rem; }
 .pb6-l { padding-bottom: 8rem; }
 .pb7-l { padding-bottom: 16rem; }
 .pt0-l { padding-top: 0; }
 .pt1-l { padding-top: .25rem; }
 .pt2-l { padding-top: .5rem; }
 .pt3-l { padding-top: 1rem; }
 .pt4-l { padding-top: 2rem; }
 .pt5-l { padding-top: 4rem; }
 .pt6-l { padding-top: 8rem; }
 .pt7-l { padding-top: 16rem; }
 .pv0-l { padding-top: 0; padding-bottom: 0; }
 .pv1-l { padding-top: .25rem; padding-bottom: .25rem; }
 .pv2-l { padding-top: .5rem; padding-bottom: .5rem; }
 .pv3-l { padding-top: 1rem; padding-bottom: 1rem; }
 .pv4-l { padding-top: 2rem; padding-bottom: 2rem; }
 .pv5-l { padding-top: 4rem; padding-bottom: 4rem; }
 .pv6-l { padding-top: 8rem; padding-bottom: 8rem; }
 .pv7-l { padding-top: 16rem; padding-bottom: 16rem; }
 .ph0-l { padding-left: 0; padding-right: 0; }
 .ph1-l { padding-left: .25rem; padding-right: .25rem; }
 .ph2-l { padding-left: .5rem; padding-right: .5rem; }
 .ph3-l { padding-left: 1rem; padding-right: 1rem; }
 .ph4-l { padding-left: 2rem; padding-right: 2rem; }
 .ph5-l { padding-left: 4rem; padding-right: 4rem; }
 .ph6-l { padding-left: 8rem; padding-right: 8rem; }
 .ph7-l { padding-left: 16rem; padding-right: 16rem; }
 .ma0-l { margin: 0; }
 .ma1-l { margin: .25rem; }
 .ma2-l { margin: .5rem; }
 .ma3-l { margin: 1rem; }
 .ma4-l { margin: 2rem; }
 .ma5-l { margin: 4rem; }
 .ma6-l { margin: 8rem; }
 .ma7-l { margin: 16rem; }
 .ml0-l { margin-left: 0; }
 .ml1-l { margin-left: .25rem; }
 .ml2-l { margin-left: .5rem; }
 .ml3-l { margin-left: 1rem; }
 .ml4-l { margin-left: 2rem; }
 .ml5-l { margin-left: 4rem; }
 .ml6-l { margin-left: 8rem; }
 .ml7-l { margin-left: 16rem; }
 .mr0-l { margin-right: 0; }
 .mr1-l { margin-right: .25rem; }
 .mr2-l { margin-right: .5rem; }
 .mr3-l { margin-right: 1rem; }
 .mr4-l { margin-right: 2rem; }
 .mr5-l { margin-right: 4rem; }
 .mr6-l { margin-right: 8rem; }
 .mr7-l { margin-right: 16rem; }
 .mb0-l { margin-bottom: 0; }
 .mb1-l { margin-bottom: .25rem; }
 .mb2-l { margin-bottom: .5rem; }
 .mb3-l { margin-bottom: 1rem; }
 .mb4-l { margin-bottom: 2rem; }
 .mb5-l { margin-bottom: 4rem; }
 .mb6-l { margin-bottom: 8rem; }
 .mb7-l { margin-bottom: 16rem; }
 .mt0-l { margin-top: 0; }
 .mt1-l { margin-top: .25rem; }
 .mt2-l { margin-top: .5rem; }
 .mt3-l { margin-top: 1rem; }
 .mt4-l { margin-top: 2rem; }
 .mt5-l { margin-top: 4rem; }
 .mt6-l { margin-top: 8rem; }
 .mt7-l { margin-top: 16rem; }
 .mv0-l { margin-top: 0; margin-bottom: 0; }
 .mv1-l { margin-top: .25rem; margin-bottom: .25rem; }
 .mv2-l { margin-top: .5rem; margin-bottom: .5rem; }
 .mv3-l { margin-top: 1rem; margin-bottom: 1rem; }
 .mv4-l { margin-top: 2rem; margin-bottom: 2rem; }
 .mv5-l { margin-top: 4rem; margin-bottom: 4rem; }
 .mv6-l { margin-top: 8rem; margin-bottom: 8rem; }
 .mv7-l { margin-top: 16rem; margin-bottom: 16rem; }
 .mh0-l { margin-left: 0; margin-right: 0; }
 .mh1-l { margin-left: .25rem; margin-right: .25rem; }
 .mh2-l { margin-left: .5rem; margin-right: .5rem; }
 .mh3-l { margin-left: 1rem; margin-right: 1rem; }
 .mh4-l { margin-left: 2rem; margin-right: 2rem; }
 .mh5-l { margin-left: 4rem; margin-right: 4rem; }
 .mh6-l { margin-left: 8rem; margin-right: 8rem; }
 .mh7-l { margin-left: 16rem; margin-right: 16rem; }
 .dn-l { display: none; }
 .di-l { display: inline; }
 .db-l { display: block; }
 .dib-l { display: inline-block; }
 .dit-l { display: inline-table; }
 .dt-l { display: table; }
 .dtc-l { display: table-cell; }
 .dt-row-l { display: table-row; }
 .dt-row-group-l { display: table-row-group; }
 .dt-column-l { display: table-column; }
 .dt-column-group-l { display: table-column-group; }
 .dt--fixed-l { table-layout: fixed; width: 100%; }
}
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## Authors

* [mrmrs](http://mrmrs.io)
* [johno](http://johnotander.com)

## License

MIT

