<p align="center">
<img width="300" src="https://imagedelivery.net/3TbraffuDZ4aEf8KWOmI_w/8aaa6f22-d600-4f26-cda9-c9f040863400/public"/>
</p>

# JSON Hero

JSON Hero makes reading and understand JSON files easy by giving you a clean and beautiful UI packed with extra features.

- View JSON any way you'd like: Column View, Tree View, Editor View, and more.
- Automatically infers the contents of strings and provides useful previews
- Creates an inferred JSON Schema that could be used to validate your JSON
- Quickly scan related values to check for edge cases
- Search your JSON files (both keys and values)
- Keyboard accessible
- Easily sharable URLs with path support

![JSON Hero Screenshot](https://imagedelivery.net/3TbraffuDZ4aEf8KWOmI_w/0f5735b3-2421-470b-244c-7047fd77f700/public)

## Features

### Column view

Inspired by macOS Finder, Column View is a new way to browse a JSON document.

![JSON Hero Column View](https://raw.githubusercontent.com/jsonhero-io/documentation-hosting/main/images/features-columnview.gif)

It has all the features you'd expect: Keyboard navigation, Path bar, history.

It also has a nifty feature that allows you to "hold" a descendent selected and travel up through the hierarchy, and then move between siblings and view the different values found at that path. It's hard to describe, but here is an animation to help demonstrate:

![Column View - Traverse with Context](https://raw.githubusercontent.com/jsonhero-io/documentation-hosting/main/images/features-traversewithcontext.gif)

As you can see, holding the `Option` (or `Alt` key on Windows) while moving to a parent keeps the part of the document selected and shows it in context of it's surrounding JSON. Then you can traverse between items in an array and compare the values of the selection across deep hierarchy cahnges.

### Editor view

View your entire JSON document in an editor, but keep the nice previews and related values you get from the sidebar as you move around the document:

![Editor view](https://raw.githubusercontent.com/jsonhero-io/documentation-hosting/main/images/features-editorview.gif)

### Tree view

Use a traditional tree view to traverse your JSON document, with collapsible sections and keyboard shortcuts. All while keeping the nice previews:

![Tree view](https://raw.githubusercontent.com/jsonhero-io/documentation-hosting/main/images/features-treeview.gif)

### Search

Quickly open a search panel and fuzzy search your entire JSON file in milliseconds. Searches through key names, key paths, values, and even pretty formatted values (e.g. Searching for `"Dec"` will find datetime strings in the month of December.)

![Search](https://raw.githubusercontent.com/jsonhero-io/documentation-hosting/main/images/features-search.gif)

### Content Previews

JSON Hero automatically infers the content of strings and provides useful previews and properties of the value you've selected. It's "Show Don't Tell" for JSON:

#### Dates and Times

![Preview colors](https://imagedelivery.net/3TbraffuDZ4aEf8KWOmI_w/43f2c081-c09b-47db-cb10-8f15ee6a1a00/public)

#### Image URLs

![Preview colors](https://imagedelivery.net/3TbraffuDZ4aEf8KWOmI_w/8a743bd5-a065-4f7f-1262-585c39c10100/public)

#### Website URLs

![Preview websites](https://imagedelivery.net/3TbraffuDZ4aEf8KWOmI_w/cd7f2d28-2c8d-4b37-696d-e898937c3d00/public)

#### Tweet URLS

![Preview tweets](https://imagedelivery.net/3TbraffuDZ4aEf8KWOmI_w/8455e9d6-1d3e-451e-a032-f3259204ef00/public)

#### JSON URLs

![Preview JSON](https://imagedelivery.net/3TbraffuDZ4aEf8KWOmI_w/13743860-3d9c-4cac-dde9-881fba7eba00/public)

#### Colors

![Preview colors](https://imagedelivery.net/3TbraffuDZ4aEf8KWOmI_w/22e37599-c2bd-4abd-79f2-466241d17b00/public)

### Related Values

Easily see all the related values across your entire JSON document for a specific field, including any `undefined` or `null` values.

![Editor view](https://raw.githubusercontent.com/jsonhero-io/documentation-hosting/main/images/features-relatedvalues.gif)

<!-- TODO -->

### Keyboard Shortcuts

<!-- TODO -->

### Sharing

<!-- TODO -->

## Bugs and Feature Requests

Have a bug or a feature request? Feel free to [open a new issue](/issues).

You can also join our [Discord channel](https://discord.gg/ZQq6Had5nP) to hang out and discuss anything you'd like.

## Developing

To run locally, first clone the repo and install the dependencies:

```bash
git clone https://github.com/jsonhero-io/jsonhero-web.git
cd jsonhero-web
npm install
```

Then, create a file at the root of the repo called `.env` and set the `SESSION_SECRET` value:

```
SESSION_SECRET=abc123
```

Now, run `npm start` and open your browser to `http://localhost:8787`
