Cornerstone Patches (Jellybean)
==================

Cornerstone patches-for Cyanogen and AOSP

CM10 Patches have been resolved against the recent Cornerstone jellybean release.

To Apply
----------------
    
      patch -p1 < cm-10-cornerstone.patch

To Remove (ugly, sorry)
------------------
    
      rm -rf packages/apps/CS*
      repo forall -c "git reset --hard"
      repo forall -c "git clean -df"


When I have some more time to look and test, I will put together a better application/removal process.

The commits I used to resolve the conflicts between the [Official Cornerstone](https://github.com/Onskreen/cornerstone) jellybean release and the 4.1.2 CM tree can be seen at my [frameworks/base tree](https://github.com/mateor/cm_frameworks_base/tree/cm-10-cornerstone).

__Note:__This is just a patch for the framework failures, and in no way produces a woorking rom at this time...just so I don't lose it.
