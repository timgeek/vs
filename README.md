VS
==

Drupal Views Snapshot


CONTENTS OF THIS FILE
---------------------

 * Introduction
 * Installation


INTRODUCTION
------------

Views doesn't handle revision management of the view object natively.  CTools exportables
provides a manual method of exporting views, which can then be versioned within a 
traditional CVS tool.  The Features module provides the best means of version-control for
views, but non-power users aren't always comfortable with the underlying concept behind
the features module and/or aren't always comfortable with the UI.

This module aims to provide a simple means of snapshotting views and restoring from saved
snapshots.  When a view is saved via the UI, a snapshot is taken and saved to the 
database.  This module provides a tab accessible on the views edit interface which lists
existing snapshots of the view currently being edited.  Snapshots are restored by clicking
on the timestamp link.  This takes the user to the standard views import form, but with
the fields pre-loaded with the snapshot data.  Clicking save restores the view from the
selected snapshot.


INSTALLATION
------------

1. Download and unpack this module in any legitimate Drupal module directory.
2. Enable the module from the Drupal modules admin page.
3. Create a view, save the view.  A snapshot is taken.
4. Restore from the snapshot by clicking on the view's snapshot tab and then clicking
on the snapshot timestamp and then clicking save on the import form.
