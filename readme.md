# meta-toml

> instructions for using `meta.toml` file

- store meta-information
- categorize and tag
- keep track of the state of projects


🌈✨🌠🌟 [work in progress] details to change 🌟🌠✨🌈



## generalized examples

### code
```toml
title = 'coding profile'
slug = 'profile-code'
description = 'extended bio for coding profile'
type = 'code'
tags = [ 'about-me', 'profile' ]
license = 'MIT'
homepage = 'https://dym.sh/profile-code'

[data]
raw = './readme.md'

[mirrors]
github = 'https://github.com/dym-sh/dym-sh'
gitlab = 'https://gitlab.com/dym-sh/dym-sh'
codepen = 'https://codepen.io/dym-sh/pen/zYZjozZ/left/?editors=1000'
source = 'https://source.garden/dym-sh'

[log]
created = 2020-11-22
```

### graphics
```toml
title = 'asian-nasa'
description = '[injects one mirror-selfie in a NASA shirt]'
type = 'graphics'
tags = [ 'logo', 'remix' ]
license = 'CC-BY'
homepage = 'https://dym.sh/asian-nasa'

[sources-files]
figma_online = 'https://figma.com/file/UZbwZKpkPZTi2HpIsXoCjW'
figma_local = './src/asian-nasa.fig'

[cross-posts]
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
homepage = 'https://dym.sh/hello'

[data]
raw = './readme.md'

[cross-posts]
twitter = 'https://twitter.com/dym_sh/status/1405144126081933316'

[log]
published = 2021-06-16
updated = 2021-06-16
```


## tooling
- [inventory](https://github.com/dym-sh/inventory)
- [unfolder](https://github.com/dym-sh/unfolder)
