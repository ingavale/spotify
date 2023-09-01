@@ -14,6 +14,12 @@ Spotipy's full documentation is online at [Spotipy Documentation](http://spotipy
pip install spotipy
```

alternatively, for Windows users 

```bash
py -m pip install spotipy
```

or upgrade

```bash
@@ -43,6 +49,8 @@ for idx, track in enumerate(results['tracks']['items']):

import spotipy
from spotipy.oauth2 import SpotifyOAuth
