## Supported Sites For Scraping

This list is meant to keep track of which sites are already supported by existing community scrapers. And which scrapers support them. When introducting a new scraper, add the sites your scraper supports to this list in your PR. Please keep the site list in alphabetical order to keep the list tidy. If you are adding a lot of sites to the list, it may be useful to paste the sites in and then use a tool [like this](https://wordcounter.net/alphabetize) to alphabetize it.
If a scraper needs a newer stash release than the current stable/master the version info should be added in the **Needs** field.

Column names are **S**cenes, **G**allery, **M**ovies, **P**erformers.

Supported Site|Scraper| S | G | M | P |Needs|Contents
--------------|-------|:-:|:-:|:-:|:-:|:---:|:------:
1000facials.com|GammaEntertainment.yml|:heavy_check_mark:|:x:|:x:|:x:|-|-
10musume.com|10Musume.yml|:heavy_check_mark:|:x:|:x:|:x:|-|JAV
1111customsxxx.com|ChickPass.yml|:heavy_check_mark:|:x:|:x:|:x:|-|-
18eighteen.com|TheScoreGroup.yml|:heavy_check_mark:|:heavy_check_mark:|:x:|:x:|-|-
18tokyo.com|karatmedia.yml|:heavy_check_mark:|:x:|:x:|:x:|-|JAV
18vr.com|BaDoink.yml|:heavy_check_mark:|:x:|:heavy_check_mark:|:heavy_check_mark:|-|VR
1by-day.com|DDFNetwork.yml|:heavy_check_mark:|:x:|:x:|:x:|-|-
1pondo.tv|1pondo.yml|:heavy_check_mark:|:x:|:x:|:x:|-|JAV
21naturals.com|Algolia_21Naturals.yml|:heavy_check_mark:|:x:|:x:|:x:|Python|-
21roles.com|21Roles.yml|:heavy_check_mark:|:x:|:x:|:x:|CDP|-
21sextreme.com|Algolia_21Sextreme.yml|:heavy_check_mark:|:x:|:x:|:x:|Python|-
yanks.com|Yanks.yml|:heavy_check_mark:|:x:|:x:|:x:|-|-
yngr.com|YNGR.yml|:heavy_check_mark:|:x:|:x:|:x:|-|-
younganaltryouts.com|OldGoesYoung.yml|:heavy_check_mark:|:x:|:x:|:x:|-|-
youngerloverofmine.com|Mypervmom.yml|:heavy_check_mark:|:x:|:x:|:x:|-|-
youngermommy.com|Nubiles.yml|:heavy_check_mark:|:heavy_check_mark:|:x:|:x:|-|-
youngthroats.com|Teencoreclub.yml|:heavy_check_mark:|:x:|:x:|:x:|-|-
youporn.com|YouPorn.yml|:heavy_check_mark:|:x:|:x:|:x:|-|Tube Site
yourmomdoesanal.com|ThirdRockEnt.yml|:heavy_check_mark:|:x:|:x:|:x:|-|-
yourmomdoesporn.com|ThirdRockEnt.yml|:heavy_check_mark:|:x:|:x:|:x:|-|-
yummysofie.com|YummySofie.yml|:heavy_check_mark:|:x:|:x:|:x:|-|-
z-filmz-originals.com|Z-Filmz-Originals.yml|:heavy_check_mark:|:x:|:x:|:x:|-|-
zentaidolls.com|ZentaiDolls.yml|:heavy_check_mark:|:x:|:x:|:x:|-|-
zerotolerancefilms.com|Algolia_zerotolerancefilms.yml|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|:x:|Python|-
zexyvr.com|ZexyVR.yml|:heavy_check_mark:|:x:|:x:|:heavy_check_mark:|-|VR
zishy.com|Zishy.yml|:heavy_check_mark:|:heavy_check_mark:|:x:|:x:|-|-
zoiestarr.com|ChickPass.yml|:heavy_check_mark:|:x:|:x:|:x:|-|-

## Non url scrapers

The following scrapers do not support xxxByURL scraping and are not included to the above list. To keep the below list tidy please add scrapers keeping the list in alphabetical order by the .yml filename.
For each scraper a short description, an optional comment with the usage and the related PR(s) with usage details would be appreciated.

Scraper | Description | Comments | PR
--------|-------------|----------|:--:
ComicInfoXML.yml| A ComixInfo XML gallery scraper | A python scraper that looks for ComicInfo xml compatible  files in the gallery's folder/filename and parses them | [#827](https://github.com/stashapp/CommunityScrapers/pull/827)
CopyFromScene.yml| A gallery scraper that returns metadata from the first linked scene | A python scraper that returns metadata from copied scenes, first link the scene to the gallery then run the scraper on the gallery | 
CopyToGallery.yml| A scene to gallery scraper | A python scene scraper that copies metadata from a scene to the associated galleries. Can optionally (check .py file) associate and copy meta to all galleries in the same folder as the scene| [#895](https://github.com/stashapp/CommunityScrapers/pull/895)
dc-onlyfans.yml| An Onlyfans DB scene scraper | A python scraper that scrapes Only Fans scenes using the DB file (user_data.db) created from DIGITALCRIMINAL's tool | [#847](https://github.com/stashapp/CommunityScrapers/pull/847)
Filename.yml | Scrape a scenes (local) filename to set as scene title | Utility scraper useful if you've bulk updated filenames outside of stash and want the changes synced back into stash | [#1136](https://github.com/stashapp/CommunityScrapers/pull/1136)
jellyfin.yml| A Jellyfin/Emby scraper | A python scraper that uses the Jellyfin/Emby API to look for Scenes, Performers and Movies via URL, Query or Fragments. Needs the URL, API-Key and User from Jellyfin set in jellyfin.py and the URLs in jellyfin.yml adopted to your local Jelly/Emby Instance |
MindGeekAPI.yml| A sceneBy(Name\|Fragment) scraper for MindGeek network| A python scraper that queries directly the MindGeek API. For further **needed** instructions refer to the relevant PRs and have a look in the `MindGeekApi.py` file | [#711](https://github.com/stashapp/CommunityScrapers/pull/711) [#738](https://github.com/stashapp/CommunityScrapers/pull/738) [#411](https://github.com/stashapp/CommunityScrapers/pull/411)
multiscrape.yml| A performer scraper that can utilize multiple stash Performer scrapers| A python scraper that can use multiple existing performer scrapers in order to get performer meta. To configure it edit the `multiscrape.py` file|[#594](https://github.com/stashapp/CommunityScrapers/pull/594)
performer-image-by-scene.yml| A performer image scraper that gets images from scene covers | A python scraper that searches for scenes with the performer and sets the scene cover image as the performer image|[#1039](https://github.com/stashapp/CommunityScrapers/pull/1039)
performer-image-dir.yml| A performer image scraper compatible with the actress-pics repo | A python scraper that searches in a cloned actress-pics repo for performer images. Configuration and more info in `performer-image-dir.py`|[#453](https://github.com/stashapp/CommunityScrapers/pull/453)
ScrapeWithURL.yml| A sceneByFragment scraper to perform a sceneByURL scape on scenes with URLs provided | This scraper allows users to perform sceneByURL scrapes in bulk.| [#900](https://github.com/stashapp/CommunityScrapers/issues/900)
ShokoAPI.yml| A sceneByFragment scraper for [Shoko Server](https://shokoanime.com) | A sceneByFragment scraper that queries a local Shoko Server instance using the filename for scene meta. To configure it edit the `ShokoAPI.py` file| [#586](https://github.com/stashapp/CommunityScrapers/issues/586) [#628](https://github.com/stashapp/CommunityScrapers/pull/628)
stash-sqlite.yml| A performer scraper that searches a stash db file | This python scraper uses the sqlite database from another stash instance and allows you to parse performers |[#230](https://github.com/stashapp/CommunityScrapers/pull/230) [#460](https://github.com/stashapp/CommunityScrapers/pull/460)
torrent.yml| A torrent scene scraper | This python scraper parses all torrent files in the specified directory (edit `torrent.py`) for embedded metadata using the scene's title.The title can either be a file from the torrent or the filename of the .torrent file | [#358](https://github.com/stashapp/CommunityScrapers/pull/358)
xbvrdb.yml|  A scene/gallery scraper for XBVR db files| This python scraper uses the title from stash  to search the sqlite database from XBVR for metadata. You would need to  copy `main.db` from your xbvr configuration and move this to `scrapers/xbvr.db` | [#190](https://github.com/stashapp/CommunityScrapers/pull/190)
