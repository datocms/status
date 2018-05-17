# DatoCMS Status page

## Managing incidents

Incidents are plain markdown files inside the `site/content/incidents` directory.

### Creating new incidents

Adding incidents to your status page is as simple as adding a new document to the incidents collection.
Create a new incident using npm:

```
npm run new-incident
```

You'll be asked a series of questions about the incident, then Hugo will generate a new file pre-filled with your responses.

After explaining the current situation in the incident, you can just push the file to GitHub. Netlify will deploy the indicent announcement for you in a matter of seconds.

### Resolving incidents

Everything will be operational again when all incidents are marked with `resolved = true` in the incident frontMatter:

```toml
+++
...
affectedsystems = ["API"]
resolved = true
+++
```


### Tracking activity

When there is an update in your incident you can track activity by inserting a timestamp with the update. For example:

```md
**Update**: We've identified the issue. {{< track "2016-11-22T14:34:00.000Z" >}}
```
