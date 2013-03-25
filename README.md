LwcMultipleChoice
=======
Version 0.0.1 Created by John Behrens

Introduction
------------

LwcMultipleChoice is an Zend Framework 2 Module created as example of how to combine ZF2 and Doctrine.





Requirements
------------

* [Zend Framework 2](https://github.com/zendframework/zf2) (latest master)
* [ZfcUser] (latest master).
* [Doctrine-ORM-Module] (latest master).

Features / Goals
----------------

* Provice  [COMPLETE]
* User registration [COMPLETE]
* Forms protected against CSRF [COMPLETE]
* Out-of-the-box support for Doctrine2 _and_ Zend\Db [COMPLETE]
* Registration form protected with CAPTCHA [IN PROGRESS] \(Needs more options\)
* Robust event system to allow for extending [IN PROGRESS]
* Support for additional authentication mechanisms via plugins (Google,
  Facebook, LDAP, etc) [INCOMPLETE]
* Optional E-mail address verification [INCOMPLETE]
* Forgot Password [INCOMPLETE]
* Provide ActionController plugin and view helper [INCOMPLETE]

Installation
------------

### Main Setup

#### By cloning project

1. Install the [ZfcBase](https://github.com/ZF-Commons/ZfcBase) ZF2 module
   by cloning it into `./vendor/`.
2. Clone this project into your `./vendor/` directory.

#### With composer
1. Add Repositorie to Composer.json

   "repositories": [ {
            "type": "vcs",
            "url": "https://github.com/WebconsultsEU/LwcMultipleChoice.git"
    }],
    ....
  "require": {
        ....
        "lewildecode/LwcMultipleChoice" : "dev-master"
        ....
    }
2. Now tell composer to download ZfcUser by running the command:

    ```bash
    $ php composer.phar update
    ```


3. Install the database structure
    data/structure.sql to your sql server

4. copy config/doctrine.php.dist as doctirne.php to your projects config dir
   and change your database details



#### Post installation
available sites

route /testadmin is the admin channel


Security
-----------------

At the moment any ZfcUser registered user can edit at the moment,
autohorization will be changed in further projects

