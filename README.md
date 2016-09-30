# go-jsoncommentstrip
[![GoDoc](https://godoc.org/github.com/RaveNoX/go-jsoncommentstrip?status.svg)](https://godoc.org/github.com/RaveNoX/go-jsoncommentstrip)

GO library for strip JSON comments from input.

## Comment Types

### Single Line

```json
{  
  // this is a comment
  "not_a_comment": "// this is not a comment"  
}
```


### Multiple Lines

```json
[
  /* multi
   line
   "comment",
   */
   "value": "this is not comment" /* this is another comment */
]
```

## Escaping in JSON
```json
{
    "test": "\"valid string // /*" // escaped string
}
```

## Line Endings Support
Library normally working with *NIX `\n` and Windows `\r\n` line endings.

## License
(MIT)[LICENSE.MD]