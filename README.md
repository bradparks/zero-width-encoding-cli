# zero-width-encoding-cli (`zwe`)

[![npm version](https://badge.fury.io/js/zero-width-encoding-cli.svg)](https://badge.fury.io/js/zero-width-encoding-cli)

A **Node.js** command-line application (`zwe`) to encode and decode messages 
with zero-width characters. Built off of [umpox/zero-width-detection][original]

## Installation

```
# Install with npm
npm install -g zero-width-encoding-cli

# Install with yarn
yarn global add zero-width-encoding-cli
```

## Usage

Use the `-e` flag to encode a message.

```
# Linux
zwe -e "hello world" | xclip -selection c

# macOS
zwe -e "hello world" | pbcopy
```

Use the `-d` flag to decode a message.
```
zwe -d "‌﻿​﻿​﻿‌﻿​﻿‌﻿‌﻿‌﻿‍﻿‌﻿​﻿​﻿‌﻿‌﻿​﻿‌﻿​﻿‍﻿‌﻿​﻿​﻿‌﻿​﻿​﻿‌﻿‌﻿‍﻿‌﻿​﻿​﻿‌﻿​﻿​﻿‌﻿‌﻿‍﻿‌﻿​﻿​﻿‌﻿​﻿​﻿​﻿​﻿‍﻿‌﻿‌﻿​﻿‌﻿‌﻿‌﻿‌﻿‌﻿‍﻿‌﻿​﻿​﻿​﻿‌﻿​﻿​﻿​﻿‍﻿‌﻿​﻿​﻿‌﻿​﻿​﻿​﻿​﻿‍﻿‌﻿​﻿​﻿​﻿‌﻿‌﻿​﻿‌﻿‍﻿‌﻿​﻿​﻿‌﻿​﻿​﻿‌﻿‌﻿‍﻿‌﻿​﻿​﻿‌﻿‌﻿​﻿‌﻿‌"
# => hello world
```

[original]: https://github.com/umpox/zero-width-detection
