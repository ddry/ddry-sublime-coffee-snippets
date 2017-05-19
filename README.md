# Sublime Text CoffeeScript snippets for ddry

<img src="https://cloud.githubusercontent.com/assets/5163953/22628172/6b91f120-ebe0-11e6-8456-0f5b2dc3a553.png" alt="ddry logo" width="250">

Set of CoffeeScript snippets for [ddry](https://www.npmjs.com/package/ddry) data-driven DRY Node JS testing wrapper.

Scope of all these snippets is `source:coffee`, so please save your brand new data-driven spec file as `.coffee` to enable them.

Then, even if you haven't decided yet what are you going to test, **ddp** `tab` will expand to

```coffee
'use strict'

module.exports = (dd) ->
  dd.drive [
    dd.pending()
  ]
```

This spec is very promising since it can actually engage every test harness, but sadly useless.

To start actual testing expand **dd** `tab` **it** `tab` to

```coffee
'use strict'

module.exports = (dd) ->
  dd.drive [
    it: 'get things done'
    i: [ input ]
    e: expected
  ]
```

Then `cit` will give you comma and the next `it` object, so please start it at correct indent level.

Use `ddr` to start just `dd.drive` call, `ddc` for `dd.context`. And we have now only minor snippets left.

### Matchers

`m:` for `matcher: 'plain'`
`m:a` for `matcherL 'anyOrder'`
`m:c` for `matcher: 'contains'`
`m:e` for `matcher: 'error'`
`m:p` for `matcher: 'property'`

### Hooks

`bh` for `before` hook
`ah` for `after` hook

Keep focused and save your time.
