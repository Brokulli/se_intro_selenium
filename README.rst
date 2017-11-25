=========================
Example App with Selenium
=========================

Development
===========

1. Setup the virtualenv or use the existing:

   - Prepare the coding environment with python2

     ::

       # you need to have the virtualenvwrapper installed
       # sudo pip install -U  virtualenvwrapper
       source /usr/bin/virtualenvwrapper.sh
       mkvirtualenv wsb-simple-selenium
       pip install -r test_requirements.txt

   - Continue working with virtualenv:

     ::

       workon wsb-simple-selenium

2. Install the deps if needed:

   ::

     pip install -r requirements.txt

3. Get the driver:

   - chrome (check https://sites.google.com/a/chromium.org/chromedriver/):

     ::

       wget https://chromedriver.storage.googleapis.com/2.33/chromedriver_linux64.zip
       unzip chromedriver_linux64.zip

   - firefox:

     ::

       wget https://github.com/mozilla/geckodriver/releases/download/v0.19.1/geckodriver-v0.19.1-linux64.tar.gz
       tar -xvzf geckodriver*tar.gz
       chmod +x geckodriver*
       export PATH=$PATH:$(pwd)/geckodriver

Uruchamianie
============

::

  export PATH=$PATH:$(pwd)
  python auto_search.py
