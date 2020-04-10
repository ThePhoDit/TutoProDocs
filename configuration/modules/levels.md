# Levels

This module is where you are going to manage the permissions that users have over the bot. These levels will be used as permissions to run commands and as permissions to check who can run actions over other users.

You can use users and roles IDs. Keep in mind that users IDs override roles ones. Remember that all IDs go between quotes.

Here you have an example of how a simple configuration would look like. In this case, you can change the IDs and the levels, and you can add as many as you want.

```yaml
levels:
  '459649180969730050': 150 # Owner ID
  '627156480595853322': 100 # Administrator Role
  '627241194753359931': 50  # Moderator Role
  '627241150817763380': 20  # Support Member Role
```

{% hint style="info" %}
Adding comments \(everything written after a \#\) can keep your configuration clean and more readable for everyone.
{% endhint %}



