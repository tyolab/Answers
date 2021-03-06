## 1. About ##
The Answers extension is a collection of extensions and other tools (including
a skin) to operate a questions and answers wiki with MediaWiki as the backend.

## 2. History ##
The tools were written by various Wikia developers for Wikia.

The initial public release (http://trac.wikia-code.com/changeset/39697) of the
Answers extension was on 22 July 2011, though some components of it (such as
the old skin, EditResearch extension, etc.) had been public from the very
beginning.

It appears that Wikia stopped working on the extension(s) at some point, after
which the work was picked up by Jack Phoenix <<jack@countervandalism.net>>, the
author of this very README file.

## 3. Authors ##
* Adrian Wieczorek <<adi3ek@wikia-inc.com>>
* Bartek Łapiński <<bartek@wikia-inc.com>>
* Christian Williams <<christian@wikia-inc.com>>
* David Pean <<david.pean@gmail.com>>
* Maciej Brencz <<macbre@wikia-inc.com>>
* Maciej Błaszkowski <<marooned@wikia-inc.com>>
* Nick Sullivan <<nick@sullivanflock.com>>
* Sean Colombo <<sean.colombo@gmail.com>>
* Jack Phoenix <<jack@countervandalism.net>>
* George Barnick <<george.barnick@brickcraft.me>>

## 4. On directory structure ##
The original release contained only the directories "FacebookConnect",
"templates" and "tests". I moved some other Answers-specific stuff here in an
attempt to keep things centralized.

* api
    * MediaWiki API modules, called by various things
* CategoryHubs
* EditResearch
* FacebookConnect
* FlexibleCategoryViewer
* GetQuestionWidget
    * allows users to get a question widget for their site
* maintenance
    * maintenance scripts intended to be run from command line (CLI)
* NewSkin
    * Answers skin (both old and new versions), its images, CSS and JS files
* SuperDeduper
* templates
* tests

## 5. Installing ##
Add the following to your wiki's LocalSettings.php:

```php
require_once("$IP/extensions/Answers/Answers.php");
```

After that, go to your wiki's ```[[Special:Version]]``` page to verify that the
installation was successful.
