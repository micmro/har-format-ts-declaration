# har-format-ts-declaration
TypeScript definitions (aka typings) for the HAR (HTTP Archive) file format (version 1.2).

# Usage

## Installation
The typings are on NPM, so you can simply:
```
npm install --save @types/har-format
```

## Example usage
```Typescript
import { Har } from "har-format";

function getNonRedirectEntries(file: Har){
    return file.log.entries.filter(e => !e.response.redirectURL);
}
```

Originally based on the HAR typings created for [PerfCascade](https://github.com/micmro/PerfCascade).

## Specs and resources
- [W3C HAR Spec](https://w3c.github.io/web-performance/specs/HAR/Overview.html)
- [HAR 1.2 Spec](http://www.softwareishard.com/blog/har-12-spec)
