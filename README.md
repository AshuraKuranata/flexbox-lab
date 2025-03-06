# flexbox-lab

## Introduction

The purpose of this lab is to become familiarized with the usage and handling of more complex CSS functions and to utilize Flexbox in CSS styling to better manage the designs of a web page.

Over the course of this lab, I will try to push regular content updates as each user story/situation is implemented that includes footnotes or asides to the solution as problems or research is done to catalog the journey.

## Initial & Final design

Per the instructions, this is the site that we are starting with:
<img src="https://github.com/AshuraKuranata/flexbox-lab/blob/main/images/Initial%20design.png">

And the expected outcome should look like:
<img src="https://github.com/AshuraKuranata/flexbox-lab/blob/main/images/Final%20Design.png">

After taking a look at the <a href="https://pages.git.generalassemb.ly/modular-curriculum-all-courses/flexbox-lab-solution/">live link example</a>, I noticed a few major items to track for design:

1. Certain elements would shrink and wrap, where others would not
2. No adjustments to the default main-axis or the cross-axis
3. Initial look only identified 3 sections, but at closer review after reading the recommended approach the 4th zone of the sub-nav made more sense as a 4th section to manage

The recommended approach to dealing with the web site and lab are to break it down into 4 distinct sections:

* Top Nav
* The Hero Content
* Sub-Nav
* Main Content

I will be following the recommended approach steps of adjusting the CSS stylesheet to complete this lab exercise.

## User Story 1: I want the destinations and actions in the Top Nav bar to be in a row no matter how small the screen is.

Error 1: Trying to set up flex, I kept naming it "position: flex" when I needed to do "display: flex".  Fixed issue!

Once I got flex set up for the items, I got stuck trying to figure out how to shift the alignment of the "div #actions" over to the right side of the nav bar without creating additional div classes or IDs (tried align-self: right & flex-end, justify-content: right & flex-end) and many other iterations.

After trying to research and figure it out, I connected with team member Angel who reminded me of the use of "space-between", which solved the issue.[^1]

Once this was handled, the rest of the nav bar exercise of spacing was quickly resolved.

[^1]: I'd like to research later into how to individually move child flex items within a parent container because I think it should work, and with the use case of the possibility that there might be multiple containers that you want to stack at the ends in different iterations
i.e. |12     345|

## User Story 2: I want the Hero section to have the text elements better spaced out, the search to be prominently displayed inthe middle, and for the trending items to be listed below the search all within rows.

