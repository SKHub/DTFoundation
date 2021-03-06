Change Log
==========

This is the history of version updates.

**Version 1.5.1**

- ADDED: Ability to uncompress individual files in DTZipArchive
- ADDED: DTFolderMonitor for watching a folder for changes
- ADDED: DTZipArchive Demo demonstrating DTZipArchive and DTFolderMonitor on iOS
- ADDED: DTLog logging hooks
- CHANGED: DTHTMLParser now aggregates parsed characters into a single delegate call-back
- CHANGED: Removed UIKit dependency for DTAsyncFileDeleter so that it can be moved to Core sub-spec

**Version 1.5.0**

- CHANGED: DTASN1 Moved to sub-spec, out of Core
- CHANGED: DTScripting classes moved to sub-spec, out of Core
- CHANGED: DTAlertView, DTActionSheet, UIView+DTActionHandlers moved to UIKit_BlocksAdditions sub-spec, out of UIKit
- CHANGED: Moved DTDebug methods for UIColor and UIView into sub-folder, no spec
- CHANGED: Moved Obj-C runtime methods to sub-folder, no spec
- ADDED: DTAWS for communicating with Amazon Web Services
- ADDED: Method on DTSmartPagingScrollView for accessing a specific page's view
- FIXED: Typo on DTHTMLParser sub-spec
- FIXED: Parsing the OS X version string was incorrect in DTVersion
- FIXED: DTExtendedFileAttributes was using hard-coded length for buffer

Note: While there are no breaking API changes the podspec cleanup will probably require updating your dependencies if you use projects that directly or indirectly depend on DTFoundation.

**Version 1.4.4**

- FIXED: Warning for incomplete section pragma in DTActionSheet
- FIXED: Added missing zLib dependency to PodSpec
- FIXED: DTWeakSupport.h can now also be imported into non-ARC source files
- FIXED: DTWeakSupport header missing from public headers for iOS Static Framework target
- FIXED: Removed duplicate classes from side panel demo which are already included in lib

**Version 1.4.3**

- FIXED: Removed Error in DTWeakSupport, as including this in non-ARC project is legitimate use

**Version 1.4.2**

- ADDED: DTWeakSupport.h for tagging variables and properties to use weak refs if supported
- FIXED: [DTSidePanel] classes missing from static library target
- CHANGED: Implemented conditional weak support in DTSidePanelController, DTActionSheet, DTAlertView, 
DTSmartPagingScrollView, DTHTMLParser, DTASN1Parser

**Version 1.4.1**

- ADDED: [DTCustomColoredAccessory] Added left arrow disclosure indicator
- ADDED: [DTReachability] Demo App
- CHANGED: [DTReachability] to observe reachability to apple.com instead of general IP connectivity as this addresses some issues where DNS resolving might lag behind
- FIXED: [DTSidePanel] Appearance Notifications not sent to replaced panels

**Version 1.4**

- ADDED: [DTSidePanel] Container Controller
- ADDED: [DTSQLite] Wrapper class for SQLite3 Databases
- ADDED: [DTAlertView] Method to create a cancel button and/or set a cancelBlock.
- CHANGED: Moved experimental striped layer into Experimental folder

**Version 1.3**

- ADDED: [DTReachability]
- FIXED: [DTZipArchive] Incorrect Define

**Version 1.2**

- ADDED: [DTASN1] BitString support
- ADDED: [DTASN1] DTASN1Serialization
- ADDED: [DTASN1] IA5 String support
- FIXED: [DTZipArchive] Unit Tests

**Version 1.1**

- CHANGED: Refactored base64 methods into DTBase64Coding
- ADDED: UIView Debug methods to catch errors where UIView methods are called on background thread
- ADDED: [Experimental] DTStripedLayer
- ADDED: Method to produce random color
- ADDED: DTTiledLayerWithoutFade
- ADDED: CGRectCenter
- FIXED: [AppKit] Fixed bugs in panel presenting
- CHANGED: [DTZipArchive] Various Improvements
- CHANGED: [DTUTI] Moved to separate library/subspec
- REMOVED: DTDownload and DTBonjour, they become their own repositories
