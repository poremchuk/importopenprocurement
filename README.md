OpenProcurement API to SQL bridge, Windows
Get it from https://github.com/imaginal/openprocurement.transfuse
==========

command line tool

Can be used with databases:
* SqliteDatabase
* PostgresqlDatabase
* MySQLDatabase

Usage
----------

    usage: transfuse.py [-h] [--offset OFFSET] [--limit LIMIT] [--resume]
                        base.ini [tender.ini lots.ini ...]


Requirements
----------

* Python 2.7
* virtualenv


Installation
----------

    # clone repository

    git clone https://github.com/imaginal/openprocurement.transfuse.git
    cd openprocurement.transfuse

    # setup and activate python virtualenv

    virtualenv env
    . env/bin/activate

    # install requirements

    pip install -r requirements.txt

    # edit base config

    nano base.ini

    # first run

    python transfuse.py base.ini tenders.ini --limit 10
