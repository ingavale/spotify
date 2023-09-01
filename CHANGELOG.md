# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## Unreleased

### Changed
- Changes the YouTube video link for authentication tutorial (the old video was in low definition, the new one is in high definition)
- Updated links to Spotify in documentation 


### Added
- Added optional `encoder_cls` argument to `CacheFileHandler`, which overwrite default encoder for token before writing to disk
- Integration tests for searching multiple types in multiple markets (non-user endpoints)
- Publish to PyPI action

### Fixed
- Fixed the regex for matching playlist URIs with the format spotify:user:USERNAME:playlist:PLAYLISTID.
- `search_markets` now factors the counts of all types in the `total`  rather than just the first type ([#534](https://github.com/spotipy-dev/spotipy/issues/534))



- playlist_tracks example code no longer prints extra characters on final loop iteration
- SpotifyException now thrown when a request fails & has no response ([#571](https://github.com/plamere/spotipy/issues/571), [#581](https://github.com/plamere/spotipy/issues/581))
- Added scope, `playlist-read-private`, to examples that access user playlists using the spotipy api: current_user_playlists() ([#591](https://github.com/plamere/spotipy/issues/591))
- Enable retries for POST, DELETE, PUT ([#577](https://github.com/plamere/spotipy/issues/577))

