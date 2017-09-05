## Scrapy with face_recognition

The scrapy container with face_recognition

## usage

```shell
$ docker run -it -v ~/code/python:/py annatarhe/scrapy:v0.2 /bin/bash
```

You can do this in your code:

```python
from PIL import Image
import face_recognition
import urllib.request

avatarUrl = "https://avatars3.githubusercontent.com/u/72467?v=4&s=460"

image = face_recognition.load_image_file(urllib.request.urlopen(avatarUrl))

locations = face_recognition.face_locations(image)

print(len(locations))
```

And this container include **Scrapy**!