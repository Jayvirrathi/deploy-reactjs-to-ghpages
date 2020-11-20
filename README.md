## Deploy ReactJS app to gh-pages

This Action will automate the process of building and depolying reactjs app to gh-pages.

## Action

Add this action inside your Github Repository's Actions

```
name: React app deployment

on:
  push:
    branches: [ master ]
  pull_request:
    branches: [ master ]

jobs:
  build:

    runs-on: ubuntu-latest

    steps:
    - uses: actions/checkout@v2.3.4

    - name: Deploy react app to github pages
      uses: jayvirathi/deploy-reactjs-to-ghpages@v1.0.0
```
