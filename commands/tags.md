---
description: Tags are like custom commands you can use to provide information.
---

# Tags

You can choose who can use tags inside the [Commands module](../configuration/modules/commands.md). Just use the same syntax, utilizing `use_tags` as a command name. It should look something like this:

```yaml
use_tags:
  permission: 10
  enabled: true
  disabled_channels: []
```

This works in the exact same way as the rest of commands do.

Now that you know how to control who can use your tags, let's see some useful commands:

### Get a list of tags:  \(40\)

```text
;taglist
---------
;listtag
```

### Create a tag:  \(100\)

```text
;createtag {name} {content}
---------
;addtag {name} {content}
```

### Edit a tag: \(100\)

```text
;changetag {name/id} {new content}
---------
;edittag {name/id} {new content}
```

### Delete a tag:  \(100\)

```text
;deletetag {name/id}
---------
;deltag {name/id}
```

### Fetch information about a tag:  \(40\)

```text
;infotag {name/id}
---------
;taginfo {name/id}
```

