.. title: Topcoder
.. slug: topcoder
.. date: 2015-07-13 16:50:07 UTC-04:00
.. tags: gtest, cookiecutter, topcoder
.. category: 
.. link: 
.. description: How I work on topcoder problems locally. 
.. type: text

I've only recently came across topcoder, a site where you can develop your
programming and design skills. They provide a UI to practice coding
and to compete in speed and code-quality challenges. It's a fine
interface, but I'd rather code in my own environment. I've developed a
scaffold that helps me work these  
problems out on my on machine. A scaffold-ed project has a CMake
configuration file, a stubbed class to complete the 
problem and an executable that drives a series GTest-based tests. The
tests match the examples provided in each problem description. Ideally
I would create a scraper that would pull all the values down from the site
automagically, but for now I populate some of the details
manually. `Take a
look<https://github.com/yannpaul/cookiecutter-gtest>`_ for yourself. 
