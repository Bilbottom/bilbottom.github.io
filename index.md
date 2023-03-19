<head>
  <title>Personal Projects</title>
  <link rel="shortcut icon" type="image/x-icon" href="favicon.ico?">
</head>


🚀 Personal Projects
---

## [📝 Timesheet automation with pop-up boxes](https://github.com/Bilbottom/daily-tracker)

###### [https://github.com/Bilbottom/daily-tracker](https://github.com/Bilbottom/daily-tracker)

Not sure where all your time goes? I wasn't either, so this application generates a pop-up box every 15 minutes (configurable) for me to entry what I'm working on

<div style="text-align: center;">

<img alt="pop-up-box" src="https://raw.githubusercontent.com/Bilbottom/daily-tracker/main/tracker-form-tkinter.png"/>

</div>

### ✨ Features

- Drop-down box to select from recent tasks
- Auto-populates the detail text box with the tasks' last entry
- Integrates with [Outlook <img alt="Microsoft Outlook" height="14px" src="https://outlook.live.com/favicon.ico"/>](https://outlook.live.com/owa/)
  - Reads the calendar and auto-fills with meeting information
- Integrates with [Jira <img alt="Jira Software" height="12px" src="https://example.atlassian.net/favicon.ico">](https://www.atlassian.com/software/jira)
  - Reads tickets in the current sprint and adds them to the task drop-down
  - Adds a worklog to the ticket when the form is submitted
- Integrates with [Slack <img alt="Slack" height="12px" src="https://slack.com/favicon.ico"/>](https://slack.com/)
  - Posts a message to channel when the form is submitted


### ⚠️ Warnings

- This is still very early in development and is undergoing a significant restructure
- The code coverage is extremely limited
- The Outlook integration on MacOS doesn't work for recurring meetings


---

## [<img alt="dbt-labs" height="18px" src="https://www.getdbt.com/favicon.ico"> Life Admin using dbt](https://github.com/Bilbottom/billiam-database)

###### [https://github.com/Bilbottom/billiam-database](https://github.com/Bilbottom/billiam-database)

In addition to my 'automated' timesheet (the project above), I also keep track of every transaction I make at an item level (since 2018-01-18)

This project is both a [dbt](https://www.getdbt.com/) proof-of-concept, plus a means for me to analyse my spending and work

Current lineage diagram:

<img alt="lineage-diagrams" src="https://raw.githubusercontent.com/Bilbottom/billiam-database/main/src/assets/dbt-dag.png"/>

The dbt documentation is hosted at:

- [https://bilbottom.github.io/billiam-database](https://bilbottom.github.io/billiam-database)


---

## [<img alt="PyCharm" height="20px" src="https://upload.wikimedia.org/wikipedia/commons/1/1d/PyCharm_Icon.svg"> Custom PyCharm Database Extensions](https://github.com/Bilbottom/pycharm-extensions)

###### [https://github.com/Bilbottom/pycharm-extensions](https://github.com/Bilbottom/pycharm-extensions)

PyCharm is awesome, and it's even more awesome when you write your own database extensions 😉

The repo adds 4 aggregator extensions and 2 extractor extensions:

- **Aggregators**
  - [COUNT_CHARS.groovy](https://github.com/Bilbottom/pycharm-extensions/blob/master/data/aggregators/COUNT_CHARS.groovy)
  - [COUNT_DISTINCT.groovy](https://github.com/Bilbottom/pycharm-extensions/blob/master/data/aggregators/COUNT_DISTINCT.groovy)
  - [COUNT_NULLS.groovy](https://github.com/Bilbottom/pycharm-extensions/blob/master/data/aggregators/COUNT_NULLS.groovy)
  - [HAS_BAD_CHARS.groovy](https://github.com/Bilbottom/pycharm-extensions/blob/master/data/aggregators/HAS_BAD_CHARS.groovy)
- **Extractors**
  - [One-Row.sql.groovy](https://github.com/Bilbottom/pycharm-extensions/blob/master/data/extractors/One-Row.sql.groovy)
  - [SQL-Where.sql.groovy](https://github.com/Bilbottom/pycharm-extensions/blob/master/data/extractors/SQL-Where.sql.groovy)

---

## [<img alt="Microsoft Excel" height="18px" src="https://www.microsoft.com/favicon.ico"> Custom Excel Add-In](https://github.com/Bilbottom/vba-projects/tree/main/personal-toolkit)

###### [https://github.com/Bilbottom/vba-projects/tree/main/personal-toolkit](https://github.com/Bilbottom/vba-projects/tree/main/personal-toolkit)

Excel will never go away... So let's enriched it with some quality-of-life features wrapped up into a handy custom ribbon tab (in addition to the millions of features that Excel already has).

[//]: # (Uncomment once the repo is no longer private)

[//]: # (<div style="text-align: center;">)

[//]: # ()
[//]: # (<img alt="personal-toolkit-ribbon" src="https://raw.githubusercontent.com/Bilbottom/vba-projects/main/personal-toolkit/personal-toolkit-ribbon.png"/>)

[//]: # ()
[//]: # (</div>)

The features are built using VBA and the custom ribbon tab is added using the **Office RibbonX Editor** available at:

- [https://github.com/fernandreu/office-ribbonx-editor](https://github.com/fernandreu/office-ribbonx-editor)


---

## [📘 VBA Guide](https://github.com/Bilbottom/vba-guide)

###### [https://github.com/Bilbottom/vba-guide](https://github.com/Bilbottom/vba-guide)

> This will probably not be updated any more

Can you tell I like VBA? Well, I want you to like it too -- so this is a reference material for getting started with VBA. The guide is written in LaTeX, but you can find the latest compiled version at:

- https://github.com/Bilbottom/vba-guide/blob/main/compiled/vba-guide.pdf

It was originally written for some former colleagues and has been slightly adapted for a more general audience, but probably not enough. If you want to see some VBA videos, I strongly recommend [the WiseOwl YouTube](https://www.youtube.com/@WiseOwlTutorials) tutorials:

- [https://youtube.com/playlist?list=PLNIs-AWhQzckr8Dgmgb3akx_gFMnpxTN5](https://youtube.com/playlist?list=PLNIs-AWhQzckr8Dgmgb3akx_gFMnpxTN5)
- [https://youtube.com/playlist?list=PLNIs-AWhQzckV9rAM3yv8ym4pioIMA0UR](https://youtube.com/playlist?list=PLNIs-AWhQzckV9rAM3yv8ym4pioIMA0UR)


---

## [🃏 Blackjack Emulator](https://github.com/Bilbottom/blackjack)

###### [https://github.com/Bilbottom/blackjack](https://github.com/Bilbottom/blackjack)

Blackjack can be a fun casino game to play, especially when you win. This is an attempt to build Blackjack with Python just to get familiar with OOP concepts


---

## [🔁 Mathematics Textbook on Algebraic Permutations](https://github.com/Bilbottom/permutations)

###### [https://github.com/Bilbottom/permutations](https://github.com/Bilbottom/permutations)

> Not really in development any more (and not even finished)

There's a branch of Maths called Linear Algebra, and one of the concepts that you can study is _permutations_:

- https://en.wikipedia.org/wiki/Permutation

They're a pretty simple concept, but learning about them becomes a pain because there's a lot of different --- and in some places, contradictory --- notation used to describe them and what they can do

The purpose of this project was to show all the different notations, where they differ, and how to solve problems using each of them
