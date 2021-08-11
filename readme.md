# meta-toml

> instructions for using `meta.toml` file

- store meta-information
- categorize and tag
- keep track of the state of projects



## idea

readme-files can became an infinitely-growing kitchen-sinks of information, its a place for free-form _content_.

`meta.toml` focuses on providing only _data_. it's the «github's sidebar» for projects of any kind of media (see [examples](#examples)).

for now, this is a «spec by example» draft, growing/evolving in parallel with its practical usage.
so, 🌈✨🌠🌟 [work in progress] details to change 🌟🌠✨🌈



## use

atm, just copy an example `.toml` file into your project's folder, and change all the things to fit your needs.

additional functionality like sync/mirroring/cross-posting should be provided by external tools.


### tooling
(everything is still in early stages or incomplete – this is just a place for future references)

- [project-creator](https://github.com/dym-sh/project-creator)
- [inventory](https://github.com/dym-sh/inventory)
- [unfolder](https://github.com/dym-sh/unfolder)
- [source.garden](https://github.com/source-garden/)



## examples

### [text](./examples/text.toml)
```toml
title = 'hello'
media-type = 'text'
category = 'note'
tags = [ 'bash', 'code' ]
license = 'CC-BY'
homepage = 'https://dym.sh/hello'


[data]
type = 'markdown'
raw = './readme.md'


[cross-posts]
twitter = 'https://twitter.com/dym_sh/status/1405144126081933316'


[log]
published = 2021-06-16
```


### [graphics](./examples/graphics.toml)
```toml
title = 'Asian Nasa'
slug = 'asian-nasa'
description = '[injects one mirror-selfie in a NASA shirt]'
media-type = 'graphics'
category = 'identity'
tags = [ 'logo', 'parody' ]
license = 'CC-BY'
homepage = 'https://dym.sh/asian-nasa'


[source]
figma-online = 'https://figma.com/community/file/1004406910324312767'
figma-offline = './src/asian-nasa.fig'


[cross-posts]
reddit = 'https://reddit.com/r/dym_sh/comments/nv1mzc'
twitter = 'https://twitter.com/dym_sh/status/1402223317449388033'
instagram = 'https://instagram.com/p/CP221EjHLRZ'
dribbble = 'https://dribbble.com/shots/16169327'


[[references]]
type = 'inspiration'
description = 'mirrored NASA t-shirt'
url = 'https://reddit.com/r/intermittentfasting/comments/nur2pt'
local = './ref/mirror-selfie.jpg'

[[references]]
type = 'original'
description = 'nasa meatball'
url = 'https://commons.wikimedia.org/wiki/File:NASA_logo.svg'
local = './ref/nasa-logo.svg'


[log]
created = 2021-06-08
```


### [code](./examples/code.toml)
```toml
title = 'Coding Profile'
slug = 'coding-profile'
description = 'extended bio for coding profile'
media-type = 'code'
category = 'about'
tags = [ 'self', 'resume' ]
license = 'MIT'
homepage = 'https://dym.sh/coding-profile'
source = 'https://source.garden/coding-profile'


[mirrors]
github = 'https://github.com/dym-sh/dym-sh'
gitlab = 'https://gitlab.com/dym-sh/dym-sh'


[[data]]
type = 'markdown'
raw = './readme.md'

[[data]]
type = 'plaintext'
raw = './plain.txt'


[[sync]]
name = 'codepen'
url = 'https://codepen.io/dym-sh/pen/zYZjozZ/left/?editors=1000'
data = 'markdown'

[[sync]]
name = 'hashnode'
url = 'https://hashnode.com/@dym_sh'
data = 'plaintext'


[log]
init = 2021-06-05
updated = 2021-08-04
```
