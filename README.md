# Migration Tool For Adobe Lightroom Catalogs

## Rationale

Having been a long time Lightroom user for photography, on buying a new camera my licensed copy would no longer work. Not wanting to go down the subscription route, I felt the Linux tooling (Digikam, Darktable, RawTherapee, ART, GIMP) had finally matured enough to make the leap which has been working well. 

This still left the matter of an archive of around 50000 images that had been tagged and processed. The correct thing to do would at the time would have been to export the sidecars in Lightroom itself, but I'd already removed it and Adobe of course no longer provided the installer to download because that'd be too straightforward. The goals of this project will be as follows:

* Parse the interesting file data from the SQLite catalog including primarily:
  * Keywords
  * IPTC and EXIF data
  * Ratings
  * Colour labels
  * Picks
* Write these to a sidecar file that will be compatible with Digikam and initially ART

It may be possible to extract basic processing operations (crop, white balance, exposure adjustment etc.) and add these so that they're applied, but this falls under the "nice to have" category
