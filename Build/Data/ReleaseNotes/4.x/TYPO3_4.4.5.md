Release Notes for TYPO3 4.4.5
=============================

This document contains information about TYPO3 version 4.4.5 which was
released on December 16, 2010.

News
----

This release is a combined bugfix and security release.

Notes
-----

Due to several security issues found in the TYPO3 Core, there was a
combined release of TYPO3 4.2.16, 4.3.9 and 4.4.5.\
Find more details in the security bulletin:
<https://typo3.org/teams/security/security-bulletins/typo3-sa-2010-022/>

Download
--------

<https://typo3.org/download/>

MD5 checksums
-------------

    61a6db9a29cc327c9657dbf79c8c1254  dummy-4.4.5.tar.gz
    9543933b8fdd4f36ea6663a6242af09d  dummy-4.4.5.zip
    a226de5ca324134ebc9effbed5fadc79  typo3_src-4.4.5.tar.gz
    453f1d4fb5810d75341e9037ae09a22d  typo3_src-4.4.5.zip
    c90b30bee3abc447887a17bbf99130a3  typo3_src+dummy-4.4.5.zip

Upgrading
---------

The usual upgrading procedure applies; no database updates are
necessary.

Changelog
---------

    2010-12-16  Oliver Hader  <oliver.hader@typo3.org>

        * Release of TYPO3 4.4.5

    2010-12-16  Oliver Hader  <oliver@typo3.org>

        * Fixed bug #14402: XSS in Install tool (thanks to Benjamin Mack)
        * Fixed bug #16590: t3lib_TSparser::checkIncludeLines() does not check files to be included (thanks to Fabrizio Branca)
        * Fixed bug #15737: quoteStrForLike does not properly escape strings in sql_mode NO_BACKSLASH_ESCAPES
        * Fixed bug #16653: SQL injection problem in class.db_list.inc (thanks to Jigal van Hemert)
        * Fixed bug #15735: FORM content object is susceptible to XSS (thanks to Benjamin Mack)
        * Fixed bug #16362: Directory traversal attack in em_unzip
        * Fixed bug #16485: Cross-Site Scripting in showpic functionality
        * Fixed bug #16593: It is possible to bypass 'verifyFilenameAgainstDenyPattern'
        * Follow-up to bug #16593: Added unit tests

    2010-12-07  Christian Kuhn  <lolli@schwarzbu.ch>

        * Fixed bug #16696: [Caching framework] unit tests: Fatal error in t3lib_cache_backend_dbbackendTest due to call to undefined method

    2010-12-04  Stanislas Rolland  <typo3@sjbr.ca>

        * Fixed bug #16675: htmlArea RTE: Incorrect result when inserting horizontal rule in FF and WebKit

    2010-12-01  Stanislas Rolland  <typo3@sjbr.ca>

        * Fixed bug #16058: htmlArea RTE: Overlay to choose a color exceeds the viewport if many colors are defined

    2010-01-01  Oliver Hader  <oliver@typo3.org>

        * Fixed bug #16604: Changes in workspace are not shown automatically in pagetree
        * Fixed bug #15495: Pagetree fails to reload

    2010-11-30  Steffen Gebert  <steffen@steffen-gebert.de>

        * Fixed bug #16581: Make jsFooterInline & jsFooterLibs available to render-preProcess hook (Thanks to Morton Jonuschat)

    2010-11-30  Xavier Perseguers  <typo3@perseguers.ch>

        * Fixed bug #16501: DBAL does not support multi-column indexes in create table queries

    2010-11-30  Steffen Kamper  <steffen@typo3.org>

        * Fixed bug #16614: common.js resets TYPO3 namespace (Thanks to Peter Kühn)

    2010-11-29  Jeff Segars  <jeff@webempoweredchurch.org>

        * Fixed bug #15189: Frontend Editing edit panels are shown for content element types that cannot be edited

    2010-11-29  Francois Suter  <francois@typo3.org>

        * Fixed bug #16583: Localization overview has no color-coded status anymore

    2010-11-26  Francois Suter  <francois@typo3.org>

        * Fixed bug #16573: Register count_MENUOBJ is not properly initialized

    2010-11-26  Christian Kuhn  <lolli@schwarzbu.ch>

        * Fixed bug #16321: [scheduler] Numeric zero for representation of weekday sunday is not accepted (Thanks to Marcus Krause)
        * Fixed bug #16582: [Caching framework] Remove misleading memcached configuration example from config_default
        * Fixed bug #16317: [scheduler] Valid values generated from cron command does not contain integers only (Thanks to Marcus Krause)

    2010-11-25  Christian Kuhn  <lolli@schwarzbu.ch>

        * Fixed bug #16319: [scheduler] CronCmd class variable "values" does not contain integers only (Thanks to Marcus Krause)

    2010-11-25  Jigal van Hemert  <jigal@xs4all.nl>

        * Fixed bug #16322: Incorrect regexp in substituteMarkerArray

    2010-11-25  Stanislas Rolland  <typo3@sjbr.ca>

        * Follow-up to bug #16431: htmlArea RTE: in WebKit, clicking on image does not select it
        * Fixed bug #16571: htmlArea RTE: Configured height of link and image dialogue windows not honoured

    2010-11-24  Stanislas Rolland  <typo3@sjbr.ca>

        * Fixed bug #16124: htmlArea RTE: Links are incorrectly updated in Google Chrome

    2010-11-24  Jigal van Hemert <jigal@xs4all.nl>

        * Fixed bug #16560: Hide mod_menu of record listing in page module if not needed (Thanks to Georg Ringer)

    2010-11-23  Steffen Ritter  <typo3@steffen-ritter.net>

        * Fixed bug #16518: Extra frame after default password change, link from reports module (Thanks to Kevin Walter)
        * Fixed bug #16517: t3lib_beFunc::getRecordWSOL() does not use it's param $useDeleteClause in else branch

    2010-11-22  Jigal van Hemert <jigal@xs4all.nl>

        * Fixed bug #14974: Extra frame after default password change, link from welcome screen (Thanks to Kevin Walter)

    2010-11-19  Stanislas Rolland  <typo3@sjbr.ca>

        * Follow-up to bug #16431: htmlArea RTE: in WebKit, clicking on image does not select it

    2010-11-17  Francois Suter  <francois@typo3.org>

        * Fixed bug #16147: getRecordOverlay fetches "Versioning Preview Overlay" but does not return the fields _ORIG_uid and _ORIG_pid (Thanks to Andreas Kiessling)

    2010-11-16  Stanislas Rolland  <typo3@sjbr.ca>

        * Fixed bug #16431: htmlArea RTE: in WebKit, clicking on image does not select it
        * Fixed bug #16433: htmlArea RTE: Default action not prevented on click in status bar

    2010-11-13  Benjamin Mack  <benni@typo3.org>

        * Fixed bug #7855: IRRE doesn't save collapse/expand state of nested IRRE records
        * Fixed bug #9508: Workspace preview link should work in multidomain-environments (Thanks to Michael Klapper)

    2010-11-12  Ernesto Baschny  <ernst@cron-it.de>

        * Fixed bug #15456: Changes made by ColorPicker Wizard are not saved (Thanks to Tobias Hoevelborn)
        * Fixed bug #6001: Install Tool image tests fail when there are spaces in the path name of im_path, and auto-detection of IM under Windows improved

    2010-11-11  Stanislas Rolland  <typo3@sjbr.ca>

        * Fixed bug #16314: Incorrect use of is_dir in class.tx_rtehtmlarea_clearrtecache.php (Thanks to Juergen Deisenroth)

    2010-11-11  Christian Kuhn  <lolli@schwarzbu.ch>

        * Fixed bug #16352: [saltedpasswords] Login with bulk updated passwords from t3sec_saltedpw not working (Thanks to Marcus Krause)

    2010-11-10  Stanislas Rolland  <typo3@sjbr.ca>

        * Fixed bug #16346: htmlArea RTE: fontstyle/fontsize may raise js error on toolbar update

    2010-11-10  Steffen Gebert  <steffen@steffen-gebert.de>

        * Fixed bug #16335: Workspace Draft Records are shown in Live Workspace in some cases (Thanks to Joerg Kinast)

    2010-11-09  Ernesto Baschny  <ernst@cron-it.de>

        * Fixed bug #15184: Generation transparent images with GMENU fails (Thanks to Mathias Schreiber)

    2010-11-08  Jeff Segars  <jeff@webempoweredchurch.org>

        * Fixed bug #14901: Forgotten styling: User Name at the top misses a CSS definition (Thanks to Christopher Stelmaszyk)

    2010-11-08  Stanislas Rolland  <typo3@sjbr.ca>

        * Fixed bug #16245: htmlArea RTE: When inserting link with IE8, trailing line break is also linked
        * Updated htmlArea RTE version to 2.0.7
        * Fixed bug #16313: htmlArea RTE: WebKit does not support copy and cut commands anymore

    2010-11-06  Steffen Kamper  <steffen@typo3.org>

        * Fixed bug #15587: Bug: htmlspecialchars called twice (Thanks to Mickel Ricky)
        * Fixed bug #16214: Bug: Change value of Media(Flash) parameter (Thanks to Janos Thiele)

    2010-11-05  Steffen Gebert  <steffen@steffen-gebert.de>

        * Fixed bug #16130: buggy initialization of flash uploader when only certain file extensions are allowed (Thanks to Andreas Kiessling)

    2010-11-04  Xavier Perseguers  <typo3@perseguers.ch>

        * Fixed bug #15656: indexed_search: Template corrections of #14130 not applied to the CSS template (Thanks to Lorenz Ulrich)

    2010-11-03  Steffen Kamper  <steffen@typo3.org>

        * Fixed bug #15995: Bug: doktype limitation is not applied to alternative page languages (pages_language_overlay) (Thanks to Andreas Kiessling)

    2010-11-03  Stanislas Rolland  <typo3@sjbr.ca>

        * Fixed bug #16175: htmlArea RTE: The path of classesAnchor images are modified when saving

    2010-10-29  Christian Kuhn  <lolli@schwarzbu.ch>

        * Fixed bug #15551: [IRRE] Open all child records when opening parent records (Thanks to Sebastian Fischer)
        * Fixed bug #16140: [reports] PHP warning on missing array in reports system extension (Thanks to Rudi Meyer)

    2010-10-29  Ernesto Baschny  <ernst@cron-it.de>

        * Fixed bug #16155: t3lib_db::INSERTquery misses a space when generering the INSERT INTO statement

    2010-10-27  Ernesto Baschny  <ernst@cron-it.de>

        * Fixed bug #16135: Output of superfluous "&qout;" in title of TCEform icon for record in group of type "db" (Thanks to Sven Juergens)

    2010-10-27  Stanislas Rolland  <typo3@sjbr.ca>

        * Fixed bug #16148: htmlArea RTE: Missing cancel browser default after inserting character or emoticon

    2010-10-27  Steffen Gebert  <steffen@steffen-gebert.de>

        * Fixed bug #15503: Improve t3lib_userAuth::getCookie() (Thanks to Michael Bürgi)

    2010-10-26  Christian Kuhn  <lolli@schwarzbu.ch>

        * Fixed bug #15936: [Caching framework] Entry identifier needs to be sanitized in FileBackend

    2010-10-25  Stanislas Rolland  <typo3@sjbr.ca>

        * Fixed bug #16087: htmlArea RTE: Missing soft hyphen entity in CharacterMap

    2010-10-21  Stanislas Rolland  <typo3@sjbr.ca>

        * Follow-up to bug #15622: t3lib_TCEforms_inline registers superfluous nested level when renderFieldsOnly is set

    2010-10-20  Ernesto Baschny  <ernst@cron-it.de>

        * Fixed bug #16075: Add IfModule mod_rewrite.c to misc/advanced.htaccess

    2010-10-19  Susanne Moog  <typo3@susanne-moog.de>

        * Fixed bug #15095: The Web>Versioning view has style issues resulting in "wrong layers"
        * Fixed bug #13294: IRRE deleted combo records are still validated by TBE_EDITOR (Thanks to Marcel Greter)

    2010-10-18  Stanislas Rolland  <typo3@sjbr.ca>

        * Fixed bug #16050: htmlArea RTE: Backspacing in empty editing area may raise js error
        * Updated htmlArea RTE version to 2.0.6

    2010-10-18  Xavier Perseguers  <typo3@perseguers.ch>

        * Fixed bug #1318: 'removeTag' does not remove closing tags

    2010-10-17  Stanislas Rolland  <typo3@sjbr.ca>

        * Fixed bug #15657: IRRE: Foreign selector with groupdb won't add new items (Thanks to Thomas Maroschik)

    2010-10-17  Steffen Kamper  <steffen@typo3.org>

        * Fixed bug #15830: Sprite - IRRE record synchronization icon missing (Thanks to Stefan Galinski)

    2010-10-17  Benjamin Mack  <benni@typo3.org>

        * Fixed bug #16022: Size calculation function can only deal with integers

    2010-10-16  Benjamin Mack  <benni@typo3.org>

        * Fixed bug #14835: IRRE Move-Icon should have curser:move (Thanks to Georg Ringer)

    2010-10-15  Benjamin Mack  <benni@typo3.org>

        * Fixed bug #16005: Live workspace does not respect move-to-placeholders
        * Fixed bug #11444: Workspace Dropdown in "Workspace" -> "Review and Publish" [LIVE workspace] always shows "[Draft Workspace]" (Thanks to Robert Heel)

    2010-10-15 Steffen Kamper  <steffen@typo3.org>

        * Fixed bug #15928:#15543 Bugfix : PHP Warning in t3lib_spritemanager (Thanks to Sven Juergens)
        * Fixed bug #15822: t3lib_beFunc use $this in static methods
        * Fixed bug #15993: Bug: Felogin shouldn't show the permalogin form controls when permalogin is set to "forced on" in install tool

    2010-10-14  Benjamin Mack  <benni@typo3.org>

        * Fixed bug #103: No Plain-text List Option

    2010-10-12  Susanne Moog  <typo3@susanne-moog.de>

        * Fixed bug #15168: Template auto complete is hidden beneath next text area field

    2010-10-11  Steffen Kamper  <steffen@typo3.org>

        * Fixed bug #12376: typo3temp got filled with thousands of javascript_* files (Thanks to Georg Ringer)

    2010-10-10  Steffen Kamper  <steffen@typo3.org>

        * Fixed bug #15835: deprecationLog in console crashes output on login page
        * Fixed bug #15727: Clean-up for PageRenderer
        * Fixed bug #15690: Change text of exception in t3lib_cache_frontend_stringfrontend
        * Fixed bug #15944: Flashmessage "content_from_pid" misses page title

    2010-10-09  Steffen Kamper  <steffen@typo3.org>

        * Fixed bug #8785: TCAselectItem not working for all tables (Thanks to Sebastian  Michaelsen)
        * Fixed bug #15865 clickmenu breaks if no record set. (Thanks to Bjoern Pedersen)
        * Fixed bug #15230: Bug/Feature: Core only is able to load one specific IE6 CSS file (Thanks to Steffen Ritter)

    2010-10-06  Stanislas Rolland  <typo3@sjbr.ca>

        * Fixed bug #15858: htlmArea RTE: Stylesheet access error in Google Chrome 7
        * Fixed bug #15863: htmlArea RTE: Initialization never completes in Google Chrome 7
        * Follow-up to bug #15858: htlmArea RTE: Stylesheet access error in Google Chrome 7
        * Fixed bug #15899: htmlArea RTE: Editing area collapsed in Chrome 7
        * Fixed bug #15893: htmlArea RTE: Insufficient Check for BE / FE Context (Thanks to Ingo Renner)

    2010-10-06  Susanne Moog  <typo3@susanne-moog.de>

        *  Fixed bug #15840: Broken loading icon when loading IRRE elements (thanks to Lars Houmark)

    2010-10-06  Steffen Kamper  <steffen@typo3.org>

        * Fixed bug #15784: Resolve errors in tslib_content
