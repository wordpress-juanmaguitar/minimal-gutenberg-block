# Minimal Gutenberg Block (with build)

This repository contains a minimal block using JSX that therefore needs a `build` process to convert the JSX syntax into JS code that browsers can understand (ES5).

## Quick Start Guide

#### 1. Install dependencies

Once the repo has been cloned, install the dependencies of `minimal-gutenberg-block-build` from inside its folder

```
cd minimal-gutenberg-block-build
npm install
```

#### 2. Generate the build 

Once the depencies are installed (a `node_modules` folder should have been created), we should launch the build process to get the final version of the block that can be used from WordPress. 

```
npm build
```

#### 3. Use it in your WordPress installation 

If you have a local WordPress installation already running, you can clone the repo and launch the commands above inside the `plugins` folder of that installation. 

If not, you can use [`wp-now`](https://github.com/WordPress/playground-tools/tree/trunk/packages/wp-now) to launch a WordPress site with the plugin installed by executing from the generated folder (and from a different terminal window or tab) the following command

```
npx @wp-now/wp-now start 
```

At this point you should be able to insert the "Minimal Gutenberg Block" block into any post (after activating the plugin "Minimal Gutenberg Block Plugin") of your WordPress installation, and see how it behaves in the frontend when published.