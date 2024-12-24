# MethStreams Live Sports Playlists

MethStreams is a platform that offers free live sports streaming across selected categories. Users can stream and watch sports directly through their browser without the need for an account or subscription.

For added flexibility, this repository provides an M3U playlist featuring MethStreams's channels. With this, you can load the streams into any IPTV application that supports M3U-formatted playlists.

You can view the full list of events provided by MethStreams [here](https://href.li/?https://methstreams.com).

The latest events added to the playlist can be found [here](https://github.com/dtankdempse/methstreams-m3u/blob/main/events.txt).

## Playlist Formats

---

### Standard Playlist Information

**Playlist.m3u8**  
This is a standard M3U playlist. To use it, ensure your IPTV application supports custom headers, specifically `Referer` and `User-Agent` (optional). The Referer header is required to access the streams, and not setting it will result in a 403 error.

#### Playlist URLs
- **M3U:** `https://bit.ly/mstream-m3u1`
  
#### Guide URLs
- **EPG (XML):** `https://bit.ly/mstream-epg`

#### Required Headers
- **Referer:** `https://methstreams.com/`
---

### TiviMate Playlist Information

- **tivimate_playlist.m3u8:**  
  This playlist is specifically formatted for use with TiviMate. Simply load the URL provided in this repository into TiviMate as an "M3U Playlist." No additional setup is needed, as TiviMate automatically manages the required headers for playback.

#### Playlist URLs
  - **M3U:** `https://bit.ly/mstream-m3u2`
    
#### Guide URLs
  - **EPG (XML):** `https://bit.ly/mstream-epg`

**Headers:** *(Automatically handled by TiviMate)*
  - **Referer:** `Included`    
---

### Kodi Playlist Information    

- **kodi_playlist.m3u8:**  
  This playlist is designed for Kodi, utilizing `#KODIPROP` properties to handle the necessary stream settings, including the required headers. It is optimized for Kodi's PVR IPTV Simple Client, ensuring compatibility with your Kodi setup.

#### Playlist URLs
  - **M3U:** `https://bit.ly/mstream-m3u3`
  
#### Guide URLs
  - **EPG (XML):** `https://bit.ly/mstream-epg`

  **Headers:** *(Automatically handled by Kodi)*
  - **Referer:** `Included`      
---

### VLC Playlist Information

- **vlc_playlist.m3u8:**  
  Optimized for VLC Media Player. This playlist uses VLC-specific formatting to ensure streams play correctly, including setting the necessary headers via `#EXTVLCOPT`.

#### Playlist URLs
  - **M3U:** `https://bit.ly/mstream-m3u4`

#### Guide URLs
  - **EPG (XML):** `https://bit.ly/mstream-epg`

  **Headers:** *(Automatically handled by VLC)*
  - **Referer:** `Included`
---
## M3U Playlist Proxy

If none of these playlists work with your IPTV application, you can try using the [m3u-playlist-proxy](https://github.com/dtankdempse/m3u-playlist-proxy). This proxy acts as a middle layer to help resolve potential issues with playing the playlists, especially if your IPTV app doesn't support setting the required headers.

## Usage Instructions:

1. Choose the playlist format that suits your application or media player.
2. Add the playlist URL to your IPTV application.
3. Ensure that your application supports the required settings, such as setting the required headers for streams to play.

---

## Disclaimer:

This repository has no control over the streams, links, or the legality of the content provided by methstreams.com (including all mirror sites). It is the end user's responsibility to ensure the legal use of these streams, and we strongly recommend verifying that the content complies with the laws and regulations of your country before use.

## DMCA Notice:

This repository does not contain any video files. It simply organizes publicly accessible web links, that can be accessed by a web browser into an M3U-formatted playlist. As far as we are aware, these websites have the necessary rights from copyright holders to stream and share the content they provide. However, if you are a copyright holder and believe that any link infringes on your rights, you can request it's removal by opening an [issue](https://github.com/dtankdempse/methstreams-m3u/issues) or submitting a [pull request](https://github.com/dtankdempse/methstreams-m3u/pulls).

Please be aware that requesting the removal of a link here will not affect the content hosted on the external websites, as this repository has no control over the files or the content being provided.
