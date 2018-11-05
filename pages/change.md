---
layout: page
title: Change
permalink: /change.html
category: change
banner-heading: Suggesting Site Changes
banner-text: All of the resources on Open CDC are available to the public by CDC public health programs. If you’re part of CDC and know of data, code, or an API that isn’t on this list but should be, please add it using the directions below.
---

### How to Suggest Changes

To add a resource to this site:

1. Navigate to the appropriate list for your open resource:
   * [_data/apis.yml](https://github.com/CDCgov/opencdc/blob/master/_data/apis.yml), for application programming interfaces,
   * [_data/data.yml](https://github.com/CDCgov/opencdc/blob/master/_data/data.yml), for data, or
   * [_data/code.yml](https://github.com/CDCgov/opencdc/blob/master/_data/code.yml), for source code.
1. Click the edit (pencil) icon in the top right corner.
1. Add your information to the list in the appropriate section.
1. Click "propose file change" at the bottom of the page.
1. Click "create pull request."
1. Provide a brief description of what you're proposing.
1. Click "Create pull request."

We will first double check that your submission is accurate. Once confirmed, we will accept the change, and the site will update to make it available.

#### Example of a Change

Each of the open technology items is described by its metadata, and this metadata is used to autogenerate the html necessary for the item to show up in this site so people can find and use it.

For example, if you wanted to add a new data set called "My Sample Data Server," you would open the [_data/apis.yml](https://github.com/CDCgov/opencdc/blob/master/_data/apis.yml) file and add four new lines for your new metadata item. Make sure to set values for all elements.

```yml
- title: Data.CDC.gov
  id: data-cdc-gov
  url: https://data.cdc.gov
  tagline: "Data.CDC.gov is a repository..."
- title: My Sample Data Server
  id: some-unique-id-wont-be-displayed
  url: https://urlto.my.server.com
  tagline: "This tagline shows as the description for my new data set and will help users understand my data, so they can better use it."
```
