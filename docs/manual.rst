.. _manual:

.. raw:: html

    <br><br>

.. title:: Manual


.. raw:: html

    <center>

manual
======

.. raw:: html

    </center>
    <br>



**NAME**

    ``KONING`` - Bejaarden, Gehandicapten, Criminelen, Psychiatrische Patienten `! <source.html>`_


**SYNOPSIS**

    ::

        koning  <cmd> [key=val] [key==val]
        koningc [-i] [-v]
        koningd 


**DESCRIPTION**


    In 2018 heb ik de koning der nederlanden geinformeerd dat wat hij
    medicatie noemt in zijn "zorg" wetten niet medicatie is maar gif.
    Bewijs dat deze medicijnen gif zijn is aan de koning getoond waarna
    zijn (persoonlijke) kabinet terug heeft geschreven dat "de koning 
    kennis heeft genomen van hetgeen ik heb geschreven".


**INSTALL**

    ::

        $ pipx install koning
        $ pipx ensurepath

        <new terminal>

        $ koning srv > koning.service
        $ sudo mv *.service /etc/systemd/system/
        $ sudo systemctl enable koning --now

        joins #koning on localhost


**USAGE**

    without any argument the bot does nothing

    ::

        $ koning
        $

    see list of commands

    ::

        $ koning cmd
        cmd,req,skl,srv


    start a console

    ::

        $ koningc
        >

    start daemon

    ::

        $ koningd
        $ 


    show request to the prosecutor

    ::

        $ koning req
        Information and Evidence Unit
        Office of the Prosecutor
        Post Office Box 19519
        2500 CM The Hague
        The Netherlands


**CONFIGURATION**

    irc

    ::

        $ koning cfg server=<server>
        $ koning cfg channel=<channel>
        $ koning cfg nick=<nick>

    sasl

    ::

        $ koning pwd <nsvnick> <nspass>
        $ koning cfg password=<frompwd>

    rss

    ::

        $ koning rss <url>
        $ koning dpl <url> <item1,item2>
        $ koning rem <url>
        $ koning nme <url> <name>


**COMMANDS**

    ::

        cfg - irc configuration
        cmd - commands
        mre - displays cached output
        pwd - sasl nickserv name/pass
        req - reconsider


**SOURCE**


    source is :ref:`here <source>`


**FILES**

    ::

        ~/.koning
        ~/.local/bin/koning
        ~/.local/bin/koningc
        ~/.local/bin/koningd
        ~/.local/pipx/venvs/koning/*


**AUTHOR**

    Bart Thate <bthate@dds.nl>


**COPYRIGHT**

    ``KONING`` is Public Domain.
