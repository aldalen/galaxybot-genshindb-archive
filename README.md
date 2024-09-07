# Galaxy.Bot Database Archive
As part of the Galaxy.Bot shutdown, we have decided to open source the ymal files that formed the "database" of the application. We have also open sourced some of the internal wiki pages that describe the layout of this repo.

## Ethos of Galaxy.Bot

Galaxy.Bot was intended to provide an high quality, approachable guides to users of all levels and experience in Genshin Impact, as well as other functions like Character information, artifact rating, and more.  This data was up to date as of the 4.7 update to Genshin Impact.

## File structure

* `artifacts/` contains all artifact information
  * `artifacts/localized/` contains all artifact information per language
  * `artifacts/rater_set_lookups/` contains all artifact information for the rater to use
  * `artifacts/source_mapping.yaml` contains a mapping between artifacts and where they are found in the game world.
* `characters/` contains all character and build info
  * `characters/info/` contains character information
  * `characters/builds/` contains character builds
* `help/` contains some of the help pages shown by the bot that might be useful for those reading this archive.
* `localization/` contains all core localization files used by the bot.  The three types of files are merged together to create the main localization file per language.
  * `localization/genshin_common/` contains localization strings that are more common to genshin itself, or shared amongst multiple types of items.
* `weapons/` contains all weapon information.
  * `weapons/localized` contains weapon information localized into supported languages.
  * `weapons/*.yaml` The yaml files in the `weapons/` directory are the weapon information files that contain data on refinement, stats, etc that are not translatable.
