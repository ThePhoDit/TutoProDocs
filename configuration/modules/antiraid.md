---
description: Keep those raiders away!
---

# Antiraid

This module will help you to keep your server secure. If this module is enabled, it will kick the users that triggered it.

```yaml
antiraid:
  new_users_amount: 50
  interval: 10 # Seconds
```

Let's see what is each property for:

**New Users Amount:** the amount of users that have to join in the selected interval.

**Interval:** seconds in which the specified amount of users have to join.

{% hint style="danger" %}
This module has not been officially tested as we cannot recreate a raid. Please report any errors you may find. 
{% endhint %}

