﻿.. include:: Images.txt

.. ==================================================
.. FOR YOUR INFORMATION
.. --------------------------------------------------
.. -*- coding: utf-8 -*- with BOM.

.. ==================================================
.. DEFINE SOME TEXTROLES
.. --------------------------------------------------
.. role::   underline
.. role::   typoscript(code)
.. role::   ts(typoscript)
   :class:  typoscript
.. role::   php(code)


ChangeLog
---------

For detailed change logs, visit `https://github.com/YAG-
Gallery/yag/commits/master <https://github.com/YAG-
Gallery/yag/commits/master>`_

.. ### BEGIN~OF~TABLE ###

.. container:: table-row

   Version
         Version
   
   Changes
         Changes:


.. container:: table-row

   Version
         3.0.0
   
   Changes
         [FEATURE] Add Formular to edit item details in the backend module
         
         [FEATURE] Define your custom item meta data fields, fill them within
         the backend form and display then within the frontend
         
         [FEATURE] AlbumViewHelper now also accepts the gallery as parameter
         
         [FEATURE] YAG FAL Driver - use YAG as a digital asset management for
         images
         
         [FEATURE] Inclusion of external JS APIs now supported
         
         [FEATURE] The Lightbox Theme is now fully responsive
         
         [FEATURE] The Lightbox Theme now uses the jQuery Lightbox Magnific
         Popup, which better performs on touch devices.
         
         [FEATURE] Add a RSS Feed for the images in your album
         
         ![FEATURE] The gallery and album filter now operate in two different
         modes
         
         [FEATURE] Custom Template Paths now support format override. Just
         place another template with the according file extension alongside the
         template and add the format parameter
         
         [FEATURE] Add additional fields to the GIFBUILDERs data
         
         [FEATURE] Add ItemListJsonViewHelper to render the itemList as a json
         
         [FEATURE] Add Javscript view to retrieve a javascript view of the
         current itemlist
         
         [BUGFIX] #53534 FAL-Drivers: Make getFileInfo more versatile and
         performant
         
         [BUGFIX] Bug #53351 Call to a member function addValidator() on a non-
         object
         
         [BUGFIX] Fixed Bug #48819: File names in zip uploader
         
         [BUGFIX] Bug #51174 Updating gallery date not possible
         
         [BUGFIX] #47958 - Removed all usages of $GLOBALS[SOBE]
         
         [BUGFIX] #51894 "Build resolution file cache" doesnt work.
         
         [BUGFIX] Fix BUG #48821 - last tag can now be deleted
         
         [BUGFIX] #49204 ExternalPlugins /Socials.ts included but not longer
         needed
         
         [BUGFIX] Bug #48940 - $item is checked with instanceOf in
         ImageViewHelper
         
         [TASK] Update .gitignore
         
         [TASK] Fix Comments


.. container:: table-row

   Version
         2.5.3
   
   Changes
         [BUGFIX] Image Files are now deleted from image source directory
         
         [BUGFIX] Hide the off page item divs with an additional hidden
         container.
         
         [BUGFIX] Image Files are now deleted from image source directory


.. container:: table-row

   Version
         2.5.2
   
   Changes
         [BUGFIX] Fix bug #48339: Albums lost after sorting with Dragn Drop
         
         [BUGFIX] #48160 Context identifier cannot be only numeric - prefix a
         "c" whenever the contextIdentifier is only numeric
         
         [BUGFIX] #48319 SqlErrorException after upgrade to YAG 2.5.1 fixed
         
         [BUGFIX] #48227 Original string not translated in
         Partials/Image/LightBoxThumb.html
         
         [TASK] Visible thumbs and pre / post list use the same partial now


.. container:: table-row

   Version
         2.5.1
   
   Changes
         [BUGFIX]: itemRepository:getRandomItemUIDs: pickRandomItems based on
         whitelist. Respect enableFields on album and gallery
         
         [BUGFIX] ZipPackingService adds file extension if not configured,
         checks if itemList is empty, cleans up the download filename.
         
         [BUGFIX] Fix Zip download link should only download images of current
         album. Should only appear if current list has images.
         
         [BUGFIX] Fixes random selection of images.


.. container:: table-row

   Version
         2.5.0
   
   Changes
         [FEATURE] ZipDownload for albums
         
         [FEATURE] Replaced the multifile flash uploader (swfupload) with
         uploadify.
         
         [FEATURE] Implemented import via "directory on server" for TYPO3 6.0+
         
         [BUGFIX] Fixed Album creation for 6.1 Property Manager
         
         [BUGFIX] Adjusted ResolutionFileCacheRepository for 6.1 repositories
         
         [BUGFIX] Creation of a new gallery in 6.1 was broken due to date
         conversion error
         
         [BUGFIX] Fixed warning in HeaderInclusion utility


.. container:: table-row

   Version
         2.4.0
   
   Changes
         [TASK] Refactored MetaData Factory
         
         [TASK] Huge refactoring towards object manger usage
         
         [FEATURE] YAG now includes a social share widget. OpenGraph
         infogrmation is automatically added to the page if the facebook share
         is activated
         
         [FEATURE] Disqus commenting partial
         
         [FEATURE] Image-List can be rendered as RSS.
         
         [FEATURE] GPS Data are now parsed and available in the meta data
         
         [FEATURE] IPTC title added to the meta data
         
         [FEATURE] Image / Album / Gallery descriptions are now richtext fields
         
         [FEATURE] Javascript inclusion can now be configured by typoscript to
         header / footer and inline.
         
         [FEATURE] Using a checkbox in the YAG extension configuration, you can
         now configure YAG to flush its resolution file cache with the TYPO3
         cache clear command.
         
         [FEATURE] The download link beneath single images now sends the file
         as download while protecting it from grabbing the whole database
         
         [FEATURE] Albumlist is sortable by date
         
         [FEATURE] MetaData encoding is recognized and metadata is
         automatically encoded to UTF8
         
         [FEATURE] Improved Plugin Information
         
         [BUGFIX] Deleted Pages are not longer seletced in Backend. #46702
         
         [BUGFIX] Breadcrumb not showin "All Albums" in Album List
         
         [BUGFIX] Album title is now also linked
         
         [BUGFIX] #45073 Fixed pid detector. TYPO3 caching was not able to
         handle comments in multi-line method calls (parameters spread over
         several lines with comments in each line).
         
         [BUGFIX] Fix album / gallery count in backend list
         
         [BUGFIX] Fix RealURL caching Bug
         
         … lots of other minor bugfixes ...


.. container:: table-row

   Version
         2.3.0
   
   Changes
         ADD: UncachedItemList as PluginModeADD: Flexform configurable filter
         to pick random items from itemList (sponsored byviazenetti.de)ADD:
         Links of ImageList items can be configured via flexform to link to
         another page and trigger YAG actions there.ADD: A flag in flexform can
         be used to reset the contextADD: PagerType can be set via typoscript.
         Availabe are “default” and “delta”ADD: YAG now officially supports all
         image-Types supportet by TYPO3ADD: #44570 YAG respects
         meaningfulTempFilePrefix in resolution filenames
         
         CHG: Improved Flexform Structure
         
         Lots of code-refactoring and clean-up!
         
         FIX: XMP ParserFIX: Mimetype is now set correctlyFIX: Bug #43846
         Invalid character in TS configuration for T3 < 6.0FIX: Bug #44505 Cash
         fails with RealURL hook because of an error in the url hashingFIX: Bug
         #44517 RealURL hook won´t work when plugin is inserted into root
         pageFIX: Bug #44556 Frontend uploading: images are not saved on the
         server


.. container:: table-row

   Version
         2.2.1
   
   Changes
         Minor Bugfixes:
         
         - Removed confusing ItemList / AlbumList
         
         - Fixed some Label Bugs
         
         - Removed Delete Link in default single image view.


.. container:: table-row

   Version
         2.2.0
   
   Changes
         YAG is now compatible to TYPO3 6.0
         
         Implemented HTML5 Drag & Drop uploading.


.. container:: table-row

   Version
         2.1.0
   
   Changes
         The Backend Directory Importer now supports file mounts.
         
         Some minor changes.
         
         Fixed Bug: #42783, #43079


.. container:: table-row

   Version
         2.0.0
   
   Changes
         Major release, now supporting PIDs to store yag records.
         
         Make sure you read update section “ `Upgrading from yag 1.x.x to yag
         2.x.x
         <#1.4.5.Upgrading%20from%20YAG%201.x.x%20to%202.x.x%20|outline>`_ ”
         
         CHG: Source selector in flexform now requires PID to be selectedADD:
         #32110 access rights for galleries and albumsADD: #34477 yag asks you
         to mark page as yag folder / select yag folder if you use module on a
         page that is not a yag folder yet.ADD: Updated documentation to match
         changes in v2.0.0CHG: yag 2.0 depends on pt\_extlist 1.0.0 and
         pt\_extbase 1.0.0ADD: Frontend-Editing has been re-introducedCHG: All
         backend TypoScript is included as extension TypoScript so no inclusion
         of TypoScript is necessary anymore to work in backend.
         
         By version 2.0 we skipped compatibility with TYPO3 version 4.5! Make
         sure to update your TYPO3 version to 4.6 at least!


.. container:: table-row

   Version
         1.5.4
   
   Changes
         FIX: #41589 Fixed dependency to wrong pt\_extlist interface in 1.5.3


.. container:: table-row

   Version
         1.5.3
   
   Changes
         FIX: Fixed bug concerning deletion of albums due to missing dependency
         injection in domain models.


.. container:: table-row

   Version
         1.5.2
   
   Changes
         TER problems, no changes compared to 1.5.1


.. container:: table-row

   Version
         1.5.1
   
   Changes
         Fixed a lot of Bugs, thanks for your bug-reports and patches:
         
         #39211. Now missing directory is re-created if origs directory is
         deleted and file-not-found images
         
         can be created within this newly created directory.
         
         #37239 CSS does not align album/gallery description properly in
         frontend
         
         #39546 absRefPrefix not respected in Resource ViewHelper
         
         #34770: Problems with RealURL hook and defaultToHTMLsuffixOnPrev
         
         #35934: Random Single View tries to display not existent images.
         
         #39211: Better Error-Message if Original Images are moved
         
         #39540 Cyrillic letters are not properly saved in "Images Overview"
         
         #39006 Titles not editable in tab »edit images«
         
         #39466: Problem with result image creation in BE
         
         #38482 (Resolved): XMP-Parsing: Website is imported as Email


.. container:: table-row

   Version
         1.5.0
   
   Changes
         CHG: We now use jQuery fancybox as lightbox for the lightox theme,
         wich is also way more configurable compared to the old lightbox. The
         lightbox theme now uses squared thumbnails.
         
         FIX BUG: #34483, #34478, #34222, #33003, #32979


.. container:: table-row

   Version
         1.4.5
   
   Changes
         FIX: BUG #34166, #33905, # 33902, #32601. Thx to the bug reporters!


.. container:: table-row

   Version
         1.4.4
   
   Changes
         FIX: BUG #32769 (thx to Steffen Gebert), #32634, #32622 (thx to
         Steffen Gebert), #32623 (thx to Steffen Gebert)


.. container:: table-row

   Version
         1.4.2
   
   Changes
         FIX: BUG #32097, #32129, #32137


.. container:: table-row

   Version
         1.4.1
   
   Changes
         ADD: Bootstrap class to easily integrate YAG in a third party
         extension.
         
         ADD: Typoscript Settings can now be retrieved from
         configurationBuilder in a Javascript compliant format


.. container:: table-row

   Version
         1.4.0
   
   Changes
         ADD: ItemsPerPage can now be set via FlexFormADD: New widget „random
         image“ availableADD: Sorting of gallery list, album list and image
         list can now be set in FlexForm.FIX: Lightbox can now thumb through
         all images of an album not only paged items.FIX: Deletion of albums
         should now work again.RFT: Some code-refactoring.


.. container:: table-row

   Version
         1.3.3
   
   Changes
         FIX: Bug #31327, #31260, #31275 – made YAG compatible to V 4.6


.. container:: table-row

   Version
         1.3.2
   
   Changes
         FIX: Bug #30692, #30909


.. container:: table-row

   Version
         1.3.0/1.3.1
   
   Changes
         RFT: Removed unused controller actions from ext\_localconf.phpADD:
         Feature bulk edit for images and albumsADD: MetaData is now processed
         correctlyADD: Tags are now imported from keywordsADD: Gallery uid
         filter for filtering certain galleries in gallery listFIX: Call-time
         pass-by-reference in realUrl hookADD: Russian translation, thanks to
         Sergey AlexandrovADD: Images can now be sorted by different criteria
         in backendADD: Resolutions can be rebuild for selected themesADD:
         Status report now gives information about configuration and external
         librariesADD: Newly imported images are now always added at the end of
         the albumFIX: Sorting images in backend manually now works on each
         page individuallyFIX: Standalone template is working againDEL: Removed
         non-used import controllerADD: Filehash is now written to item on
         import. Prevention of duplicate import.FIX: Date can be set for
         gallery and album.RFT: Performance improvements in backendADD: Added
         some styling to pager in backend
         
         FIX: Many minor and major bugfixes


.. container:: table-row

   Version
         1.2.4
   
   Changes
         FIX: It was not possible to delete images.


.. container:: table-row

   Version
         1.2.3
   
   Changes
         FIX: Fixed Bug #29187, #29393, #27964


.. container:: table-row

   Version
         1.2.1
   
   Changes
         CHG: Removed unused tabs from content element formFIX: Fixed PagerFIX:
         Removed warnings that showed up in different situations


.. container:: table-row

   Version
         1.2.0
   
   Changes
         RFT: Removed pt\_tools. YAG now uses pt\_extbase for external
         tools.FIX: Fixed Bug #27319, #27737, #27312, #27370 due to non
         existing original image file


.. container:: table-row

   Version
         1.1.9
   
   Changes
         ADD: Pager partial can now be set via TSCHG: Upload button in backend
         now looks like upload button


.. container:: table-row

   Version
         1.1.8
   
   Changes
         FIX: Removed some useless var\_dump()


.. container:: table-row

   Version
         1.1.7
   
   Changes
         ADD: Resolutions for album thumb and gallery thumb can now be set
         individually


.. container:: table-row

   Version
         1.1.6
   
   Changes
         FIX: Bug #27172 – Umlaute are now correctly displayed in Front- and
         Backend.


.. container:: table-row

   Version
         1.1.5
   
   Changes
         FIX: Bug #26740 – Insert plugin in backend crashes under some
         circumstances.FIX: Bug #26111 - Fileadmin importer is not able to
         import folders with blanks


.. container:: table-row

   Version
         1.1.4
   
   Changes
         DEL: Removed RBAC installation routineFIX: Added some escaping for
         title and descriptionRFT: Added some frontend stylingCHG: Added .jpeg,
         .JPG and .JPEG as possible file endings for importersRFT: Removed
         unused gallery:album mm table from SQL definition
         
         FIX: Some minor bugfixes


.. container:: table-row

   Version
         1.1.3
   
   Changes
         CHG: Improvements in performance. Tested handling of up to 50k images.
         Seems to be quite fast now :-)CHG: Directory importer comes with
         directory picker now.CHG: ZIP import now can handle zipped
         folders.FIX: BUG #25454, fixed 1st level resolution file cache.ADD:
         Added some documentation.


.. container:: table-row

   Version
         1.1.2
   
   Changes
         CHG: Changed TypoScript structure. Previously inserted plugins still
         remain functional, but if you edit the Plugin configuration, you have
         to select your gallery / album / item again.FIX: Paging in
         SpecificAlbum mode throws an exception. You have to edit your album
         and select the mode again.CHG: Plugins now displays mode / album /
         theme in the page content element overviewCHG: Album / gallery
         description is displayed in the module


.. container:: table-row

   Version
         1.1.1
   
   Changes
         CHG: Galleries and Albums are now again sortable. (a change in the
         database was necessary!)CHG: Complete Extension is now
         translatable.ADD: Added german translation (Thanks to Matthias
         Kuchem).CHG: Add all parameters to the URL instead of using the
         stateHashCHG: Removed all tables from the list module. All data should
         be administrated by the YAG module.CHG: ReolutionFileCache-Files are
         now identified by parameter hash.
         
         FIX: Many more minor bugs.


.. container:: table-row

   Version
         1.1.0
   
   Changes
         RFT: RBAC is no longer a dependency. Features will be outsourced to
         yag\_feedit extensionFIX: German translations are removed from JS
         filesFIX: Added lots of translationsRFT: Removed lots of CSS and
         JavaScript to make Backend work better (thx to Matthias!)ADD: Page
         cache is cleared, if objects changeFIX: Thumbs are now generated on
         Windows platformsFIX: Directory import now respects filetypes
         correctlyRFT: Image processing now uses T3 standard libs and has many
         configurations now


.. container:: table-row

   Version
         1.0.10
   
   Changes
         Bugfix release


.. container:: table-row

   Version
         1.0.9
   
   Changes
         Bugfix release


.. container:: table-row

   Version
         1.0.8
   
   Changes
         FIX: Fixed some bugs concerning contextIdentifier to enable tt\_news
         integration


.. container:: table-row

   Version
         1.0.7
   
   Changes
         FIX: Multiple instances of the plugin can now be positioned on the
         same page with different themesFIX: Bug #13820 – SWUploader not
         working without FE Session. Thanks to PETIT YannFIX: Bug #13822 - No
         thumbnails are created on Windows servers. Thanks to PETIT YannADD:
         Caching has been refactoredRFT: Image ViewHelper has been moved to
         another directoryADD: Implemented automatic cache cleaning, when
         objects changeCHG: Added lazy loading for domain modelsADD: Single
         image view now has Download-Link for full-res imageADD: Documentation


.. container:: table-row

   Version
         1.0.6
   
   Changes
         ADD: Implemented cachingADD: DocumentationRFT: Reduced number of SQL
         queries in Domain Model


.. container:: table-row

   Version
         1.0.5
   
   Changes
         Problems with TER upload – no changes


.. container:: table-row

   Version
         1.0.4
   
   Changes
         ADD: DocumentationFIX: Bug #13763 / display error message when static
         template is not includedADD: Breadcrumbs show "all galleries" when
         gallery list is shownADD: Implemented pageCacheManager,
         clearAllPageCacheAction to Backend ControllerFIX: #13775 Adding a new
         album to a gallery shows right gallery nowFIX: #13776 After importing
         from directory on server, the album list is shownFIX: Fixed bug in
         directory crawler


.. container:: table-row

   Version
         1.0.3
   
   Changes
         ADD: DocumentationADD: Some translationFIX: Dependencies are set
         correctly in ext\_emconf.php


.. container:: table-row

   Version
         1.0.0
   
   Changes
         First release of this extension.


.. ###### END~OF~TABLE ######

We are currently using GitHub.com for collaborative development. You
can find all commit messages and an up-to-date trunk of this extension
on:

https://github.com/yag-gallery

If you would like to join the team, send us an e-mail (info@yag-
gallery.de)

|img-2| 74

