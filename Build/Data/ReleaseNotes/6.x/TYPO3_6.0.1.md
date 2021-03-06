Release Notes for TYPO3 6.0.1
=============================

This document contains information about TYPO3 version 6.0.1 which was
released on January 29th 2013.

News
----

This release is a bug fix release only.

Download
--------

<https://typo3.org/download/>

MD5 checksums
-------------

    6a2946621c62653cdb0ad2e1a51e5a5e  blankpackage-6.0.1.tar.gz
    5120ae81674aba87dd91d3fd36d11592  blankpackage-6.0.1.zip
    50f3be53573b465859043070d7eed3d7  dummy-6.0.1.tar.gz
    cca76d3e814209490ebb8789fd8f8f19  dummy-6.0.1.zip
    b855c47d87a67d80dbaea71ad4edf4e3  governmentpackage-6.0.1.tar.gz
    6845e45f4c263c76d17c84565d182f28  governmentpackage-6.0.1.zip
    70ee907392a31d174253503b7d30e0fa  introductionpackage-6.0.1.tar.gz
    893a1a6d782891c5ade41a0d8f4d7fc8  introductionpackage-6.0.1.zip
    c68258b0faa15b9aa34fb695f3b433fa  typo3_src+dummy-6.0.1.zip
    807e7fe7fc1bc4f2fa61a49f3af2ccc0  typo3_src-6.0.1.tar.gz
    31c657b52faefaa65c5413d313b41d86  typo3_src-6.0.1.zip

Upgrading
---------

The [usual upgrading
procedure](https://docs.typo3.org/typo3cms/InstallationGuide/) applies.
No database updates are necessary.

Changes
-------

Here is a list of what was fixed since [6.0.0](TYPO3_6.0 "wikilink"):

    2013-01-29  60ae1e8                  [RELEASE] Release of TYPO3 6.0.1 (TYPO3 Release Team)
    2013-01-29  f636a22  #44610          [BUGFIX] FLUIDTEMPLATE cObj uses wrong template file (Christian Kuhn)
    2013-01-29  cff4f93  #44895          [TASK] EXT:reports Improve xclass reporting (Christian Kuhn)
    2013-01-28  c324e40  #43726          [TASK] Remove function usage ctype_alnum in PageRenderer (Ingo Pfennigstorf)
    2013-01-28  0fe067d  #44890          [BUGFIX] tt_content: exclude config fields (Felix Kopp)
    2013-01-28  8fbfcaf  #40866          [BUGFIX] Backend groups: exclude config fields (Felix Kopp)
    2013-01-28  3ce4491  #44892          [BUGFIX] Possible warning in about module (Christian Kuhn)
    2013-01-28  5f18e7d  #44876          [BUGFIX] Make submit button save all tabs in extension manager (Jan-Erik Revsbech)
    2013-01-28  1bb9907  #44818          [TASK] EM: Refactor Configuration handling (Christian Kuhn)
    2013-01-26  4380d35                  [TASK] Raise submodule pointer (Christian Kuhn)
    2013-01-26  cdd6897  #44808          [TASK] Add cursor:pointer to inline header (Georg Ringer)
    2013-01-26  04b3f8a  #43730          [BUGFIX] Invalid description of noPHPscriptInclude (dprecup)
    2013-01-26  3329d6e  #43797          [BUGFIX] Fix error listing in belog (Tomita Militaru)
    2013-01-25  e75848a  #44526          [TASK] Use property injection in LanguageController (Sebastian Michaelsen)
    2013-01-25  5443f33  #44744          [TASK] Cleanups for sysext belog (Sebastian Michaelsen)
    2013-01-25  e31eb56  #42775          [BUGFIX] Fix problem with saving extension configuration in different tabs (Jan-Erik Revsbech)
    2013-01-25  6836c23  #44145          [BUGFIX] Correct TCA inclusion for uploads rendering (Alexander Stehlik)
    2013-01-25  5f1973b  #43856          [BUGFIX] EM: un/install visual feedback (Felix Kopp)
    2013-01-25  4dc2bd9  #44540          [BUGFIX] Avoid PHP Warning  in Page Module (Roland Waldner)
    2013-01-23  5fd986c  #44152          [TASK] Add save only button to Scheduler task (Lorenz Ulrich)
    2013-01-23  f574627  #44701          [BUGFIX] Missing subcategories labels in EM (Francois Suter)
    2013-01-23  4469dd9  #44549          [BUGFIX] IRRE forms not using full width (Ingo Renner)
    2013-01-22  529b8ad  #44718          [BUGFIX] Instantiate new classes in typo3/* files (Francois Suter)
    2013-01-19  d99c4eb  #44665          [BUGFIX] ConfigurationUtility loses extension key (Francois Suter)
    2013-01-17  2e3ad69  #43874          [BUGFIX] array_merge_recursive_overrule: __UNSET for array values (Sebastian Michaelsen)
    2013-01-16  6f7b37e  #44506          [TASK] Remove references to oldstyle Login News (TYPO3_CONF_VARS) (Sebastian Michaelsen)
    2013-01-13  99b6527  #44439          [BUGFIX] Fix incomplete mocking in ResourceStorage test (Helmut Hummel)
    2013-01-13  f15b448  #44439          [BUGFIX] Persist files that are updated in ResourceStorage (Helmut Hummel)
    2013-01-13  0263c4d  #44481          [BUGFIX] Use array in check for new CE button (Jigal van Hemert)
    2013-01-12  f3dcd93                  Revert "[BUGFIX] LocalDriver needs to respect "is_writeable"" (Helmut Hummel)
    2013-01-12  b12c82f  #43919          [BUGFIX] Fix typos in stdWrap_crop description (Markus Klein)
    2013-01-12  3074abd  #43796          [BUGFIX] Syslog error icons problem (Tomita Militaru)
    2013-01-12  2abebe6  #44470          [BUGFIX] Content elements in wrong column in page module (Oliver Hader)
    2013-01-12  bbfe1b5  #43330          [BUGFIX] BE login shows unaesthetic scrollbars (Torben Hansen)
    2013-01-12  af01ce4  #44370          [BUGFIX] LocalDriver needs to respect "is_writeable" (Georg Ringer)
    2013-01-12  aa1463e  #42882          [BUGFIX] FAL: update wizard fails if file does not exist (Andreas Wolf)
    2013-01-12  6ba6394  #42873,#42933   [BUGFIX] Problem with special character in files and folders (Christian Weiske)
    2013-01-12  21a67af  #42925          [BUGFIX] File-Upload does not sanitize umlauts in filenames (Christian Weiske)
    2013-01-12  25e9a63  #44425          [BUGFIX] Add access check in FAL renameFolder() (Georg Ringer)
    2013-01-12  719f9fe  #43676          [BUGFIX] Adjust hooks after moving/namespacing (Stefan Neufeind)
    2013-01-12  ef9f13e  #44429          [BUGFIX] Fix array_merge when creating FAL access rights (Georg Ringer)
    2013-01-12  025887d  #43668,#44312   [BUGFIX] Fix rootline translation (Helmut Hummel)
    2013-01-11  ff81594  #38135          [BUGFIX] Apc Cache backend has side effects (Daniel Pötzinger)
    2013-01-06  8f826f5  #42453          [BUGFIX] Fix shown references of files (Helmut Hummel)
    2013-01-05  da29f0c  #44242          [BUGFIX] Include file tables in access list (Helmut Hummel)
    2013-01-04  7003f86  #43425          [BUGFIX] Change localconf.php to LocalConfiguration.php (Adrian Giurgiu)
    2013-01-04  3847227  #44301          [BUGFIX] Invalid call to t3lib_TCEmain::processRemapStack() (Oliver Hader)
    2013-01-04  7edf97e                  [TASK] Raise submodule pointer (TYPO3 Release Team)
    2013-01-02  fc7d04a  #42092          [BUGFIX] Suggest wizard is behind form inputs (Xavier Perseguers)
    2013-01-01  86dd859  #44263          [BUGFIX] phpdoc: $urlParameters can be a string (Stefan Neufeind)
    2012-12-27  a731d1b  #44237          [BUGFIX] Fix erroneous replacement of language label (Helmut Hummel)
    2012-12-20  55bca03  #34964          [BUGFIX] FE session records are never removed (Steffen Müller)
    2012-12-20  f1214e9  #32278          [BUGFIX] INTincScript_loadJSCode() causes PHP warnings (Markus Klein)
    2012-12-20  22bddc3  #43426          [BUGFIX] Fix broken logo file in Install Tool (Tomita Militaru)
    2012-12-18  e8310e5  #43584          [TASK] CleanUp References to old ClassNames (Steffen Ritter)
    2012-12-18  991a38f  #43715          [BUGFIX] Missing Task.php (Philipp Gampe)
    2012-12-18  edaef65  #44051          [TASK] Fix phpDoc of BackendUtility::displayWarningMessages (Sebastian Michaelsen)
    2012-12-17  ae6318c  #44073          [BUGFIX] Update checksums after file processing (Helmut Hummel)
    2012-12-14  abe1049  #44013          [BUGFIX] Always allow access to processing folder (Helmut Hummel)
    2012-12-12  e0b8b19  #43909          [BUGFIX] Element Browser rendering hook is wrong (Oliver Hader)
    2012-12-11  a7e0253  #32605          [BUGFIX] Incorrect RTE transform of external URL with @ character (Stanislas Rolland)
    2012-12-10  2438905  #43603          [BUGFIX] Enable the RTE with WebKit version 534 on iOS and Android (Stanislas Rolland)
    2012-12-10  daba5e2  #38472          [BUGFIX] Remove HTML in RuntimeException from sysext 'install' (Philipp Gampe)
    2012-12-08  577aef1  #43766          [BUGFIX] IE9 crashes after saving with RTE (Stanislas Rolland)
    2012-12-07  db79f0f  #43484          [BUGFIX] Catch all errors in EM ViewHelper (Georg Ringer)
    2012-12-02  3aa7323                  [BUGFIX] Errorpage background color (t3skin) (Felix Kopp)
    2012-12-02  fe2efc6  #43433          [BUGFIX] Wrong category assignment in sys_note (Wouter Wolters)
    2012-12-02  9481036  #43510          [BUGFIX] Misspelled functionname in GeneralUtility (Stefan Neufeind)
    2012-12-01  dbeaa4d  #43323          [TASK] Rename bg-image (login/error) to avoid browser caching issues (Ernesto Baschny)
    2012-12-01  5aaea94  #43321          [BUGFIX] Prevent type hinting for user functions in EM configuration (Nicole Cordes)
    2012-12-01  a0032a7  #25113          [BUGFIX] Fix wrong column title in web>list for field colpos (Martin Kästner)
    2012-12-01  4e7124f  #43470          [BUGFIX] SqlParser: trim all kinds of whitespaces (Stefan Neufeind)
    2012-11-30  7642b7d  #43459          [TASK] Remove typo3.pageModule.js (Falk Kühnel)
    2012-11-30  9531c09  #43468          [BUGFIX] Fix Task examples in scheduler (Wouter Wolters)
    2012-11-30  01fd9dc  #42292          [BUGFIX] Installer: Reference images wrong (Stefan Neufeind)
    2012-11-30  6c905a6  #43473          [TASK] ext:form Unit test all filters (Andreas Lappe)
    2012-11-30  cab3ed1  #40706          [BUGFIX] Error in configuration of scheduler task (Philipp Gampe)
    2012-11-30  ef426db  #43381          [BUGFIX] ClassLoader error after installing extension (Oliver Hader)
    2012-11-30  f3fd603  #43466          [BUGFIX] Page module Drag&Drop broken (Christian Kuhn)
    2012-11-29  98eacf9  #32515          [BUGFIX] Form values with newlines escaped in email (Helmut Hummel)
    2012-11-29  23804c6  #43330          [BUGFIX] Remove BE login scrollbars (Markus Klein)
    2012-11-29  5868e1f  #43456          [BUGFIX] ContentObjectRenderer instantiates old class names (Christian Kuhn)
    2012-11-29  f6b1e09  #43460          [BUGFIX] EM does not update extension list (Helmut Hummel)
    2012-11-29  4843709                  [TASK] Activate travis also for 6.0 branch (Helmut Hummel)
    2012-11-28  0402806  #43373          [BUGFIX] HTML syntax error in login.html (Markus Klein)
    2012-11-27  ac3c16a                  [TASK] Set TYPO3 version to 6.0.1-dev (TYPO3 Release Team)
    2012-11-27  59b7d46                  [RELEASE] Release of TYPO3 6.0.0 (TYPO3 Release Team)


