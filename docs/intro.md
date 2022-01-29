---
sidebar_position: 6
---

# Welcome!

Congrats on taking the first steps to protecting your discord server.  

Sherlock is very **dynamic**.  Use the features you wish and don't worry about the rest.

Anything **unclear** or **buggy** in this tutorial? [Please report it!](https://github.com/facebook/docusaurus/discussions/4610)

- #### Going forward, it will be assumed, you have invited the bot to your server.  If you have not, please read above on how to get Sherlock to join your server.

## Step 1
- Move the role created by inviting Sherlock to the highest role allowed.  Sherlock will only be able to modify users that are not above his highest role.
- Move the "quarantine" role created by Sherlock to right below his role in the hierarchy.  This role will be called "SL-Quarantine"

## Step 2
#### Set your own bot prefix!

`/guildsetting bot-prefix !` </br>
This would set the prefix to ! for your server.

With Sherlock, You have many options at your disposal.  We don't require you to use our pre-set prefix.  We invite you to use your own so that Sherlock may fit better in your server.

## Step 3

#### Set your log channel.

`/guildsetting logging set (channel)`</br>

This setting is key to get notifications on any actions Sherlock takes as well as any important updates from the "mother-ship".</br>  
**Example Notification:**</br>
![Example](../../static/img/logexample.png)

## Step 4

#### Word Filtering!
Sherlock is equipped with two methods of filtering out words that you do not want in your server.  There is a `soft-filter` and a `hard-filter`.

### Soft Filter
The `soft-filter` allows the user to remove the filtered word from their message before its automatically deleted.  This is most useful for someone new who doesn't know that certain words aren't allowed in your server.

To **ADD** the word "kiwi" to the filter we would use the following command.</br>
`/softfilter add word:kiwi`

To **REMOVE** the word "kiwi" from the filter we would use the following command.</br>
`/softfilter remove word:kiwi`

To **LIST** all words in the soft-filter we would use the following command.</br>
`/softfilter list`

### Hard Filter
The `hard-filter` is on the opposite end of the spectrum.  Any messages that trigger this filter's actions are deleted **IMMEDIATELY** with an additional action of 3 options.  (See below)

```text
0 - Add the regular points to the HEAT system
1 - Quarantine the user for review
2 - Kick the user from the server
3 - Ban the user from the server
```

To **ADD** the word "kiwi" to the filter we would use the following command.</br>
`/hardfilter add word:kiwi action:1`

To **REMOVE** the word "kiwi" from the filter we would use the following command.</br>
`/hardfilter remove word:kiwi`

To **LIST** all words in the soft-filter we would use the following command.</br>
`/hardfilter list`

