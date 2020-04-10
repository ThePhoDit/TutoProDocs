# On Join Roles

You can assign roles to new members that join your server. Follow this example to do so:

```yaml
on_join_roles: ['630576778271784964', 'Other Role ID']
```

Another way of doing this is like this:

```yaml
on_join_roles:
  - '630576778271784964'
  - 'Other Role ID'
```

You can add as many as you want.

{% hint style="info" %}
As you have seen, there are two ways of setting up those lists. I personally prefer the seconds one, as it is much more clear, so it is the one that I will be using through all this guide.
{% endhint %}

