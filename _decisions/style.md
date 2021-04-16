---
type: decision
acronym: style-configuration
title: >
    Use SASS for style configuration  
decision_type: must
belongs_to: devops
status: _3_sig_agreed
responsible: JLÜ;JSP
deadline: 2021-03-22
implemented: partially
todos:
    
history:
    v1:
        date: 2021-03-22
        comment: created initially
---

## Why is there need for such a decision?

In order to reach a global style configuration all teams must use the same stylesheet language.

## Additional sources for better understanding the background

[SASS](https://sass-lang.com/)

[LESS](http://lesscss.org/)

[Sass(scss) vs Less](https://lightweb-media.de/tech/sass-vs-less/)

[Sass vs. Less](https://www.educba.com/sass-vs-less/) 

## Viable Options

* LESS
* Sass(Scss)

## Alternatives not seriously considered

* plain CSS

## How is this decision evaluated?

The linked sources have been reviewed and the syntax was compared with plain css which are used at this time in the project.

## Resolution Details

The pair has decided that the best option will be SASS with using SCSS Syntax.

## Reasons for the resolution

The comparison between the syntax SASS,SCSS and LESS showed that SCSS is similar to CSS syntax. The fact that the developer can choose between CSS and non-CSS syntax if the project use the SASS language is a positive effect.
