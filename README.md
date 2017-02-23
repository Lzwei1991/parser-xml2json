# Parser XML 2 JSON

Blazing fast XML parser to JSON written in Rust ([node2object](https://github.com/vorot93/node2object)).

## Requirements

- `rust`
- `cargo`

## API

### `parseString(xmlString[, options], callback)`
 - `xmlString` - A string that represents an XML
 - `options` - an optional object where:
   - `object` - Parse JSON string to Object. default `false`
 - `callback` - a function with the signature `function (err, result)`

### `parseFile(filePath[, options], callback)`
- `filePath` - Relative or absolute path to an `.xml` file
- `options` - an optional object where:
  - `object` - Parse JSON string to Object. default `false`
- `callback` - a function with the signature `function (err, result)`


## Benchmark
Results from a i7 2.2 Ghz

```
Package                 Time taken
----------------------  ----------
parser-xml2json (rust)  0.0468 s
xml2js (js)             0.1286 s
xml2json (js and c++)   0.1329 s
```

### How to run the benchmark script on your machine

```
npm i
npm i benchmark/
node benchmark/index.js
```

## License

MIT
