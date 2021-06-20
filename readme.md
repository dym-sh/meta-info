# meta-toml

> instructions for using `meta.toml` file

- store meta-information
- categorize and tag
- keep track of the state of projects


# 🌈✨🌠🌟 [work in progress] details to change 🌟🌠✨🌈


## generalized examples

### code
```toml
title = 'IndieWeb profile'
slug = 'profile-indieweb'
description = 'plans and other info about my personal website'
type = 'code'
tags = [ 'about-me', 'profile' ]
license = 'MIT'

[data]
raw = './profile.wiki'

[sync]
indieweb = 'https://indieweb.org/User:Dym.sh'

[mirrors]
github = 'https://github.com/dym-sh/profile-indieweb'
gitlab = 'https://gitlab.com/dym-sh/profile-indieweb'
source = 'https://source.garden/dym-sh/profile-indieweb'

[cross-posts]
_canonical = 'https://dym.sh/profile-indieweb'
```

### graphics
```toml
title = 'asian-nasa'
description = '[injects one mirror-selfie in a NASA shirt]'
type = 'graphics'
tags = [ 'logo', 'remix' ]
license = 'CC-BY'


[sources-files]
figma_online = 'https://figma.com/file/UZbwZKpkPZTi2HpIsXoCjW'
figma_local = './src/asian-nasa.fig'


[cross-posts]
_canonical = 'https://dym.sh/asian-nasa'
reddit = 'https://reddit.com/r/dym_sh/comments/nv1mzc'
twitter = 'https://twitter.com/dym_sh/status/1402223317449388033'
instagram = 'https://www.instagram.com/p/CP221EjHLRZ/'


[[references]]
type = 'inspiration'
description = 'mirrored NASA t-shirt'
url = 'https://reddit.com/r/intermittentfasting/comments/nur2pt'

[[references]]
type = 'original'
description = 'nasa meatball'
url = 'https://commons.wikimedia.org/wiki/File:NASA_logo.svg'


[log]
published = 2021-06-08
```


### note
```toml
title = 'hello'
type = 'note'
tags = [ 'sh', 'code' ]

[cross-posts]
_canonical = 'https://dym.sh/hello'
twitter = 'https://twitter.com/dym_sh/status/1405144126081933316'

[log]
published = 2021-06-16
updated = 2021-06-16
```


## tooling
[TBD]


## mirrors
- https://github.com/dym-sh/meta-toml
- https://gitlab.com/dym-sh/meta-toml
- https://source.garden/dym-sh/meta-toml
