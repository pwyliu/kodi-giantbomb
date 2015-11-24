# kodi-giantbomb
Giant Bomb addon for Kodi/XBMC.

## Testing
Tested on `OpenELEC 5.0.0/Kodi 14 (Helix)`.

## Installation
1. Clone the project: `git clone https://github.com/pwyliu/kodi-giantbomb.git`
2. Create a zip file of the plugin you want to install (see below)
3. Transfer zip to the system running Kodi and use 
`System->Settings->Add-Ons->Install from zip file`

### Creating a zip file
To install from a zip file, you need to create a zip archive with a name like 
`plugin.video.giantbomb-<VERSION>.zip`, where `<VERSION>` matches the version 
in `addon.xml`. The only thing allowed in the top level of the zip is the 
directory `plugin.video.giantbomb`.

On OSX do not use the compress action from Finder to create the zip, as this 
will add a directory for OSX resource forks (`__MACOSX`) to the archive. 
Instead, it's better to create the zip from the command line. For example:

```bash
git clone https://github.com/pwyliu/kodi-giantbomb.git
cd kodi-giantbomb
zip -r plugin.video.giantbomb-4.0.2.zip plugin.video.giantbomb
```
