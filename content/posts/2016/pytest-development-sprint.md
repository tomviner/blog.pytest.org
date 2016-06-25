Title: pytest development sprint
Date: 2016-06-26 09:00
Tags: sprint2016
Authors: pfctdayelise
Summary: Summary of happenings at the June 2016 development sprint.


We have just wrapped up the pytest development sprint, which was held 20-25 June 2016 in Freiburg, Germany. Other sprints have taken place at Python conferences, but this was the first dedicated standalone event. We had 27 participants from five continents!

It was funded by [an indiegogo campaign](https://www.indiegogo.com/projects/python-testing-sprint-mid-2016#/) which raised over US$12,000 with nearly 100 backers. Several companies generously donated $500 or more:

* [Dropbox](https://www.dropbox.com/home)
* [Dolby Laboratories](http://www.dolby.com/)
* [Optiver APAC](http://www.optiver.com/sydney/)
* [Splunk](http://www.splunk.com/)
* [Cobe.io](https://cobe.io/)
* [Personalkollen](https://personalkollen.se/)
* [FanDuel](https://www.fanduel.com/)

Participants travelled from around Europe and the UK, the US, Brazil, Australia and China.

Work started or finished included the following.

Discussions:

* hooks/plugin mechanics
* what to include in pytest 3.0
* tox roadmap
* [making tox work with conda environments](https://bitbucket.org/nicoddemus/tox/branch/conda-tox-design)
* process for removing deprecated features
* new 'fromcontext' scope for fixtures
* lightning talks

Major features:

* dropping pytest assert reinterpret code
* [rename binary from 'py.test' to 'pytest'](https://github.com/pytest-dev/pytest/issues/1629) (but don't worry, ``py.test`` will still work)
* [documentation restructuring](https://github.com/pytest-dev/pytest/wiki/Docs-refactor)
* [``--setup-only`` and ``--setup-plan`` flags which show how fixtures are initialised without actually running the tests](https://github.com/pytest-dev/pytest/pull/1647)
* Adding ``-o`` commandline option to override .ini config values

Other features:

* pytest-qt features - improvements towards 2.0 release
* pytest-bdd enhancements
* pytest-html enhancements
* pytest-environment research
* 4 projects [submitted](http://pytest.org/latest/contributing.html#submitting-plugins-to-pytest-dev) to pytest-dev organisation

Bugs fixed/in progress:

* [exit pytest on collection error](https://github.com/pytest-dev/pytest/issues/1421)
* [markers stain on all related classes](https://github.com/pytest-dev/pytest/issues/568)
* [removed deprecated command line options](https://github.com/pytest-dev/pytest/issues/1657)
* [incorrectly dropping brackets on display of assertions](https://github.com/pytest-dev/pytest/issues/925)
* [rename getfuncargvalue to getfixturevalue](https://github.com/pytest-dev/pytest/issues/1625)
* [warning if you use getfuncargvalue in unparametrized fixtures](https://github.com/pytest-dev/pytest/issues/460)
* [terminal newlines in failed test output](https://github.com/pytest-dev/pytest/issues/1553)
* [escaping curly braces in a tox command doesn't work](https://bitbucket.org/hpk42/tox/issues/212)
* [Tox shouldn't call pip directly to avoid shebang limitations](https://bitbucket.org/hpk42/tox/issues/66)

In total at least 29 pull requests were merged to pytest, and at least 12 to tox, not to mention many others to plugins.

![Hiking in the sunny Black Forest]({attach}images/sprint_hiking.jpg){.img-rounded}

We also spent some time designing the stickers and t-shirts. Surveys will be going out to backers who chose these perks in the fundraising campaign very soon.

Thank you so much to everyone who supported the sprint. We have greatly expanded knowledge of pytest internals, and we're looking forward to bringing you pytest 3.0 very soon (aiming for before EuroPython)!
