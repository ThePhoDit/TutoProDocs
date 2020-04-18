# Suggestions

Suggestions are an essential part of TutoPro. They allow users to upgrade communities by letting the administrators what they would like to see.

Let's see how this module is configured:

```yaml
suggestions:
  reviewing_channel: 'Channel ID 1'
  voting_channel: 'Channel ID 2'
  approved_channel: 'Channel ID 3'
  potential_channel: 'Channel ID 4'
  denied_channel: 'Channel ID 5'
```

**Reviewing Channel:** if this property has a channel ID, all new suggestions will be sent to here. The idea is that the selected channel can only be seen by moderators who first [review](../../commands/suggestions.md) the content.

**Voting Channel:** this property is necessary for the plugin to work. Suggestions are sent here once they have been reviewed or if no reviewing channel was established. Users can vote here.

**Approved Channel:** channel where [approved](../../commands/suggestions.md#approve-a-suggestion) suggestions will be sent. If it is not configured, the suggestion in the voting channel will be edited.

**Potential Channel:** channel where [potential](../../commands/suggestions.md#mark-a-suggestion-as-potential) suggestions will be sent. If it is not configured, the suggestion in the voting channel will be edited.

**Denied Channel:** channel where [denied](../../commands/suggestions.md#deny-a-suggestion) suggestions will be sent. If it is not configured, the suggestion in the voting channel will be edited.

