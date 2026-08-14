<head>
  <title>Personal Projects</title>
  <link rel="shortcut icon" type="image/x-icon" href="favicon.ico?">
</head>

<span style="font-weight:bold">🚀 Personal Projects</span>

**What's on this page?**

Showcase of some of my favourite personal projects:

* TOC
{:toc}

---

## Technical articles

During my time at [Tasman Analytics](https://www.tasman.ai), I wrote some of [their articles](https://www.tasman.ai/news):

- [8 Ways to Flex DuckDB](https://www.tasman.ai/news/8-ways-to-flex-duckdb)
- [Modern Python Development with uv](https://www.tasman.ai/news/modern-python-development-astral-uv)
- [Tasman's Top Ten Tips & Tricks for dbt](https://www.tasman.ai/news/10-essential-dbt-tips-and-tricks-for-faster-development)
- [Modern SQL: The Latest and Greatest SQL Features (part 1)](https://www.tasman.ai/news/modern-sql-the-latest-and-greatest-sql-features-part-1)
- [Modern SQL: The Latest and Greatest SQL Features (part 2)](https://www.tasman.ai/news/modern-sql-the-latest-and-greatest-sql-features-part-2)
- [Our Favourite Git Tips and Tricks](https://www.tasman.ai/news/our-favourite-git-tips-and-tricks)

---

## [<img alt="dbt Labs" height="16px" src="https://www.getdbt.com/favicon.ico"> dbt-π: Custom Python in dbt](https://github.com/billwallis/dbt-py)

<span style="color:grey" size=1>[https://github.com/billwallis/dbt-py](https://github.com/billwallis/dbt-py)</span>

dbt is great, but its use (correction: _abuse_) of Jinja is not 😭

The repo shims dbt to allow custom Python to be available as Jinja callbacks.

This makes it possible to rewrite Jinja macros as Python code, giving us:

- A better developer experience
- First-class support for unit testing
- Type hints and better control flow logic

---

## [📖 SQL Learning Materials](https://github.com/billwallis/sql-learning-materials)

<span style="color:grey" size=1>[https://github.com/billwallis/sql-learning-materials](https://github.com/billwallis/sql-learning-materials)</span>

A site where I document lots of SQL stuff:

- [https://billwallis.github.io/sql-learning-materials/](https://billwallis.github.io/sql-learning-materials/)

This has a set of _actually_ difficult SQL challenges largely based on real problems I've encountered in my career:

- [Challenging SQL problems](https://billwallis.github.io/sql-learning-materials/challenging-sql-problems/challenging-sql-problems/)

...as well as some written tutorials with corresponding YouTube videos:

- [From Excel to SQL](https://billwallis.github.io/sql-learning-materials/from-excel-to-sql/from-excel-to-sql/) ([YouTube playlist](https://www.youtube.com/playlist?list=PLEiRgvTilK5rhnVPQ_Tj3Q-CI0rGn_uiD))
- [Everything about joins](https://billwallis.github.io/sql-learning-materials/everything-about-joins/everything-about-joins/) ([YouTube playlist](https://www.youtube.com/playlist?list=PLEiRgvTilK5rJilO6gc809Eg2Qajgeh02))

---

## [⏱️ Database Query Profiler](https://github.com/billwallis/db-query-profiler)

<span style="color:grey" size=1>[https://github.com/billwallis/db-query-profiler](https://github.com/billwallis/db-query-profiler)</span>

One of the awesome things about SQL is that there are so many different ways to get the same output. One of the hardest things about SQL is knowing which way is the most performant way 😝

Enter: the **Database Query Profiler**.

This is a Python package that will run a set of queries against your database a number of times and return the average execution times. It's intended to be used during development to help you understand the actual performance of your queries.

> **_This is NOT a replacement for analysing the [query plan](https://en.wikipedia.org/wiki/Query_plan). This should just support the analysis done with it._**

**✨ Features**

- Database agnostic, just provide a class that can execute a query against your database
- Minimal setup required, drop your queries into a directory and run!
- Provides real-time feedback on the progress of the profiling (thanks to [`tqdm`](https://github.com/tqdm/tqdm))

A typical output will look something like this:

```
Start time: 2023-05-07 12:38:06.879738
----------------------------------------
100%|██████████| 5/5 [00:01<00:00,  3.29it/s]
query-1.sql: 0.10063192s (33.4%)
query-2.sql: 0.20044784s (66.6%)
----------------------------------------
End time: 2023-05-07 12:38:08.757555
```

---

## [📝 Timesheet automation with pop-up boxes](https://github.com/billwallis/daily-tracker)

<span style="color:grey" size=1>[https://github.com/billwallis/daily-tracker](https://github.com/billwallis/daily-tracker)</span>

Not sure where all your time goes? I wasn't either, so this application generates a pop-up box every 15 minutes (configurable) for me to enter what I'm working on.

<div style="text-align: center;">

<img alt="pop-up-box" src="https://raw.githubusercontent.com/billwallis/daily-tracker/main/tracker-form-tkinter.png"/>

</div>
<br>

> [!WARNING]
>
> This is a work in progress. I'm currently using it to track my time, but it's not yet ready for public consumption.

**✨ Features**

- Drop-down box to select from recent projects
- Drop-down box to select the selected project's recent details
- By default, autopopulates the project and details from the previous entry
- Integrates with:
  - [Google Calendar <img alt="Google Calendar" height="12px" src="https://calendar.google.com/googlecalendar/images/favicons_2020q4/calendar_28.ico"/>](https://calendar.google.com/)
  - [Outlook <img alt="Microsoft Outlook" height="14px" src="https://outlook.live.com/favicon.ico"/>](https://outlook.live.com/owa/)
  - [Jira <img alt="Jira Software" height="12px" src="https://example.atlassian.net/favicon.ico">](https://www.atlassian.com/software/jira)
  - [Slack <img alt="Slack" height="12px" src="https://slack.com/favicon.ico"/>](https://slack.com/)
  - [GitHub <img alt="GitHub" height="12px" src="https://github.com/favicon.ico"/>](https://github.com/)
  - [Monday.com <img alt="Monday.com" height="12px" src="https://monday.com/favicon.ico"/>](https://monday.com/)

---

## [<img alt="pre-commit" height="16px" src="https://pre-commit.com/favicon.ico"> Bill's Hooks](https://github.com/billwallis/bills-hooks)

<span style="color:grey" size=1>[https://github.com/billwallis/bills-hooks](https://github.com/billwallis/bills-hooks)</span>

I love [pre-commit](https://pre-commit.com/), and I've been building out some of my own hooks.

Current available hooks:

- `check-filename-pattern`: Check that filename match a specified regular expression
- `check-no-commit-comment`: Check for `NO_COMMIT` comments
- `tidy-gitkeep`: Remove redundant `.gitkeep` files

There is also the undocumented hook `check-dbt-project-version` which keeps the version specified in `dbt_project.yml` in sync with the Python project version.

---

## [<img alt="Advent of Code" height="16px" src="https://adventofcode.com/favicon.ico"> Advent of Code (SQL)](https://github.com/billwallis/advent-of-code-sql)

<span style="color:grey" size=1>[https://github.com/billwallis/advent-of-code-sql](https://github.com/billwallis/advent-of-code-sql)</span>

Solutions to the Advent of Code problem sets, written in SQL!

My DSA isn't great so I don't have any complete years yet, but it's a fun way to flex [DuckDB](https://duckdb.org/).

---

## [🥋 SQL Problems](https://github.com/billwallis/sql-problems)

<span style="color:grey" size=1>[https://github.com/billwallis/sql-problems](https://github.com/billwallis/sql-problems)</span>

There are countless websites for practising SQL. I've attempted the hardest free problems across a bunch of them, documenting [my solutions](https://github.com/billwallis/sql-problems/tree/main/src) and [my opinions on the platforms](https://github.com/billwallis/sql-problems/blob/main/src/reviews.md).

---

## [<img alt="PyCharm" height="16px" src="https://upload.wikimedia.org/wikipedia/commons/1/1d/PyCharm_Icon.svg"> Custom PyCharm Database Extensions](https://github.com/billwallis/pycharm-extensions)

<span style="color:grey" size=1>[https://github.com/billwallis/pycharm-extensions](https://github.com/billwallis/pycharm-extensions)</span>

PyCharm is awesome, and it's even more awesome when you write your own database extensions 😉

The repo adds four aggregator extensions and three extractor extensions:

- **Aggregators**
  - [COUNT_CHARS.groovy](https://github.com/billwallis/pycharm-extensions/blob/main/pycharm-extensions/data/aggregators/COUNT_CHARS.groovy)
  - [COUNT_DISTINCT.groovy](https://github.com/billwallis/pycharm-extensions/blob/main/pycharm-extensions/data/aggregators/COUNT_DISTINCT.groovy)
  - [COUNT_NULLS.groovy](https://github.com/billwallis/pycharm-extensions/blob/main/pycharm-extensions/data/aggregators/COUNT_NULLS.groovy)
  - [HAS_BAD_CHARS.groovy](https://github.com/billwallis/pycharm-extensions/blob/main/pycharm-extensions/data/aggregators/HAS_BAD_CHARS.groovy)
- **Extractors**
  - [Jira-Server.md.groovy](https://github.com/billwallis/pycharm-extensions/blob/main/pycharm-extensions/data/extractors/Jira-Server.md.groovy)
  - [One-Row.sql.groovy](https://github.com/billwallis/pycharm-extensions/blob/main/pycharm-extensions/data/extractors/One-Row.sql.groovy)
  - [SQL-Where.sql.groovy](https://github.com/billwallis/pycharm-extensions/blob/main/pycharm-extensions/data/extractors/SQL-Where.sql.groovy) (deprecated)

---

## [<img alt="Microsoft Excel" height="16px" src="https://www.microsoft.com/favicon.ico"> Custom Excel Add-In](https://github.com/billwallis/vba-projects/tree/main/personal-toolkit)

<span style="color:grey" size=1>[https://github.com/billwallis/vba-projects/tree/main/personal-toolkit](https://github.com/billwallis/vba-projects/tree/main/personal-toolkit)</span>

Excel will never go away... So let's enrich it with some quality-of-life features wrapped up into a handy custom ribbon tab (in addition to the millions of features that Excel already has).

<div style="text-align: center;">

<img alt="personal-toolkit-ribbon" src="https://raw.githubusercontent.com/billwallis/vba-projects/main/personal-toolkit/personal-toolkit-ribbon.png"/>

</div>


The features are built using VBA, and the custom ribbon tab is added using the **Office RibbonX Editor** available at:

- [https://github.com/fernandreu/office-ribbonx-editor](https://github.com/fernandreu/office-ribbonx-editor)

---

## [📘 VBA Guide](https://github.com/billwallis/vba-guide)

<span style="color:grey" size=1>[https://github.com/billwallis/vba-guide](https://github.com/billwallis/vba-guide)</span>

> This will probably not be updated any more

Can you tell that I like VBA? Well, I want you to like it too: this is a reference material for getting started with VBA. The guide is written in LaTeX, but you can find the latest compiled version at:

- [https://github.com/billwallis/vba-guide/blob/main/compiled/vba-guide.pdf](https://github.com/billwallis/vba-guide/blob/main/compiled/vba-guide.pdf)

It was originally written for some former colleagues and has been slightly adapted for a more general audience, but probably not enough. If you want to see some VBA videos, I strongly recommend [the WiseOwl YouTube](https://www.youtube.com/@WiseOwlTutorials) tutorials:

- [https://youtube.com/playlist?list=PLNIs-AWhQzckr8Dgmgb3akx_gFMnpxTN5](https://youtube.com/playlist?list=PLNIs-AWhQzckr8Dgmgb3akx_gFMnpxTN5)
- [https://youtube.com/playlist?list=PLNIs-AWhQzckV9rAM3yv8ym4pioIMA0UR](https://youtube.com/playlist?list=PLNIs-AWhQzckV9rAM3yv8ym4pioIMA0UR)

---

## [🧑‍🎓 Master's Dissertation Graphs](https://github.com/billwallis/ma5p1-dissertation-code)

<span style="color:grey" size=1>[https://github.com/billwallis/ma5p1-dissertation-code](https://github.com/billwallis/ma5p1-dissertation-code)</span>

> Originally an R project, this has been reduced and reworked as a Python project

As part of my dissertation, I was exploring ["point-line duality"](<https://en.wikipedia.org/wiki/Duality_(projective_geometry)>) -- and it was easiest to do this by drawing up the points and the lines using a computer.

One of the images has also been used as the thumbnail for the song **Perdidos en la Multitud** by the Argentinian musician **Aroldo De Souza**:

- [https://www.instagram.com/aroldo_de_souza/](https://www.instagram.com/aroldo_de_souza/)
- [https://open.spotify.com/track/5XXUJO0EzWpjkRpvrkZkt1?si=2ebc3c24556b44ff](https://open.spotify.com/track/5XXUJO0EzWpjkRpvrkZkt1?si=2ebc3c24556b44ff)

The description to go with this image is:

> In Mathematics, there is a concept of point-line duality: that is, for a point on a graph there is a corresponding line called its _dual_. The dual of the point `(a, b)` is the set of points `{(x, y)}` such that `ax + by = 0`, and we call the set of points a _line_.
>
> An interesting consequence of this duality is that if a collection of points all line on a straight line, then their dual lines will all intersect in the same place. The image is the duals of some points on the cubic curve `y = x^3`. The points on the cubic curve have been selected so that there are many sets of 3 points that all lie on the same line (such as `(-1, -1)`, `(0, 0)`, and `(1, 1)`) which means that their duals (the lines) have many intersections of exactly three lines.

If you look carefully, you'll also see that the image has been set as the tab icon for this page 😉

<br>
<div style="text-align: center;">

<img alt="cubic-graph-61" src="favicon.ico"/>

</div>
