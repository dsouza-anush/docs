# Media assets

Use this folder to organize screenshots, diagrams, and videos referenced in the documentation.

## Directory structure

```
media/
  images/
    ai-studio/       # Screenshots specific to AI Studio docs
    heroku-vibes/    # Screenshots used in Heroku Vibes docs
    shared/          # Images that appear across multiple sections
  videos/            # MP4/WebM clips embedded in docs
```

Add new subdirectories as other areas of the docs gain dedicated assets (for example `media/images/model-context-protocol/`). Keep filenames lowercase and hyphenated for clarity, e.g. `setup-flow.png` or `home.mp4`.

## Referencing images in MDX

Import the file using a relative path from the MDX file and wrap it with a `<Frame>` for consistent styling:

```mdx
import Image from "next/image";

<Frame>
  <Image
    src="/media/images/heroku-vibes/home.png"
    alt="Heroku Vibes home screen"
    width={1280}
    height={720}
    priority
  />
</Frame>
```

For static `<img>` tags you can use:

```mdx
<img src="/media/images/ai-studio/tools.png" alt="AI Studio tools" />
```

## Referencing videos

Store MP4/WebM files in `media/videos/` and embed them with the `<Video>` component:

```mdx
import { Video } from "@mintlify/components";

<Video src="/media/videos/heroku-vibes/transfer-flow.mp4" poster="/media/images/heroku-vibes/app.png" />
```

Remember to commit both the media file and any documentation changes together so the links remain valid.
