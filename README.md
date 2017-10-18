# FeedPoster Sample

An example custom integration that automates posting new articles into a predefined Workplace group when new content appears on a given RSS feed.

*FeedPoster requires the **Manage group content** permission*

## Setup
1. Create a new [Custom Integration](https://developers.facebook.com/docs/workplace/custom-integrations) app with **Manage group content** permission.
2. Check out the code and deploy to a server capable of hosting [node.js](https://nodejs.org) applications.
3. Run `npm install` to install the required modules
4. Modify the `.env` file to include the `ACCESS_TOKEN` for your app, the group ID for your `TARGET_GROUP` and a URL for the RSS feed you want to use, and start the node application by running `node clock.js`

## Notes on Cron
This app uses the `cron` module for scheduling. Visit the [cron project page](https://www.npmjs.com/package/cron) for details on how to use it for custom scheduling.
