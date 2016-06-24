Title: pytest development sprint
Date: 2016-06-26 09:00
Tags: sprint2016
Authors: pfctdayelise
Summary: Summary of happenings at the June 2016 development sprint.


We have just wrapped up the pytest development sprint, which was held 20-25 June 2016 in Freiburg, Germany. Other sprints have taken place at Python conferences, but this was the first dedicated standalone event. We had more than 20 participants from four continents!

It was funded by [an indiegogo campaign](https://www.indiegogo.com/projects/python-testing-sprint-mid-2016#/) which raised over US$12,000 with nearly 100 backers. Several companies generously donated more $500 or more:

* [Dropbox](https://www.dropbox.com/home)
* [Dolby Laboratories](http://www.dolby.com/)
* [Optiver APAC](http://www.optiver.com/sydney/)
* [Splunk](http://www.splunk.com/)
* [Cobe.io](https://cobe.io/)
* [Personalkollen](https://personalkollen.se/)
* [FanDuel](https://www.fanduel.com/)

Participants travelled from around Europe and the UK, the US, Brazil and Australia.

Work started or finished included the following.

Discussions:

* hooks/plugin mechanics
* what to include in pytest 3.0
* tox roadmap
* [making tox work with conda environments](https://bitbucket.org/nicoddemus/tox/branch/conda-tox-design)
* process for removing deprecated features
* lightning talks

Major features:

* dropping pytest assert reinterpret code
* [rename binary from 'py.test' to 'pytest'](https://github.com/pytest-dev/pytest/issues/1629)
* documentation restructuring
* ``--setup-only`` flag which shows how fixtures are initialised without actually running the tests

Bugs fixed:
*
*
