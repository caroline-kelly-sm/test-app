# test-app

This will serve a dummy Vue application that uses SUI design system.

## Running locally

### Prerequisites
- First four points in [Cloud Computing Environment Checklist](https://siteminder.atlassian.net/wiki/spaces/eng/pages/602051554/Cloud+Computing+Environment+Checklist#CloudComputingEnvironmentChecklist-nvmandNodeJS)


### Setup
```
// Fork this repo or clone directly
// git clone git@github.com:paula-abella/test-app.git

// Go to the project directory
cd test-app

// Install dependencies
npm install

// Run the application locally
npm run serve
```

Then go to http://localhost:8080/

You should see the following:

<img width="720px" alt="test-app-demo" src="https://user-images.githubusercontent.com/84423488/174955650-633f1a29-56c1-489d-85c2-90c4e130f8ca.png">

This dummy application has the navigation and some testing pages setup.
It's meant to serve a simple and static page so it's not using any of our BEEF architecture.

### Updating packages
To bump the SUI libraries to get the latest version(s)

```
npm i @siteminder/sui-core@latest @siteminder/sui-icons@latest @siteminder/sui-themes@latest
```

### Using the components
To update existing pages in the application, open up any of the views.

For example, open `src/views/direct-booking/direct-booking-rates.vue` then add HTML directly into the `template` tag.
Note that in Vue, there should be one root element, for example an outer `div` with all the contents inside.

```html
<template>
  <div>
    <!-- One root div element above or any other element then add the rest of the elements here -->
  </div>
</template>
```

The CSS styles can go in the `style` tag. We use SCSS pre-processing.

```html
<style lang="scss" scoped>

/* CSS goes here */

</style>
```
