---
title: Browser extensions
slug: Mozilla/Add-ons/WebExtensions
page-type: landing-page
sidebar: addonsidebar
---

Extensions, or add-ons, can modify and enhance the capability of a browser. Extensions for Firefox are built using the WebExtensions API cross-browser technology.

The technology for extensions in Firefox is, to a large extent, compatible with the [extension API](https://developer.chrome.com/docs/extensions/reference/) supported by Chromium-based browsers (such as Google Chrome, Microsoft Edge, Opera, Vivaldi). In most cases, extensions written for Chromium-based browsers run in Firefox with [just a few changes](https://extensionworkshop.com/documentation/develop/porting-a-google-chrome-extension/).

## Key resources

- Guides
  - : Whether you're just beginning or looking for more advanced advice, learn about how extensions work and use the WebExtensions API from our extensive range of [tutorials and guides](/en-US/docs/Mozilla/Add-ons/WebExtensions/What_are_WebExtensions).
- References
  - : Get comprehensive details about the methods, properties, types, and events of the [WebExtensions APIs](/en-US/docs/Mozilla/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs) and full details about the [manifest keys](/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json).
- Firefox workflow
  - : Discover how to build and publish extensions for Firefox: get the lowdown on developer tools, publication and distribution, and porting on [Extension Workshop](https://extensionworkshop.com/).

> [!NOTE]
> If you have ideas or questions or need help, you can reach us on the [community forum](https://discourse.mozilla.org/c/add-ons/35) or in the [Add-ons Room](https://matrix.to/#/#addons:mozilla.org) on [Matrix](https://wiki.mozilla.org/Matrix).

## Get started

Discover [what extensions can do](/en-US/docs/Mozilla/Add-ons/WebExtensions/What_are_WebExtensions) before building [your first extension](/en-US/docs/Mozilla/Add-ons/WebExtensions/Your_first_WebExtension) and [your second extension](/en-US/docs/Mozilla/Add-ons/WebExtensions/Your_second_WebExtension). Learn about the [anatomy of an extension](/en-US/docs/Mozilla/Add-ons/WebExtensions/Anatomy_of_a_WebExtension) and get an overview of the [extension development and publication workflow, Firefox style](https://extensionworkshop.com/documentation/develop/firefox-workflow-overview/). Explore a little deeper with a comprehensive selection of [example extensions](/en-US/docs/Mozilla/Add-ons/WebExtensions/Examples) that you can run right in Firefox. Continue your learning by [discovering a list of resources](/en-US/docs/Mozilla/Add-ons/WebExtensions/What_next) to follow.

## Concepts

Get detailed information on the concepts that underpin extensions.

- [Overview of the JavaScript API](/en-US/docs/Mozilla/Add-ons/WebExtensions/API)
- [Content scripts](/en-US/docs/Mozilla/Add-ons/WebExtensions/Content_scripts)
- [Background scripts](/en-US/docs/Mozilla/Add-ons/WebExtensions/Background_scripts)
- [Match patterns](/en-US/docs/Mozilla/Add-ons/WebExtensions/Match_patterns)
- [Working with files](/en-US/docs/Mozilla/Add-ons/WebExtensions/Working_with_files)
- [Internationalization](/en-US/docs/Mozilla/Add-ons/WebExtensions/Internationalization)
- [Content security policy](/en-US/docs/Mozilla/Add-ons/WebExtensions/Content_Security_Policy)
- [Native messaging](/en-US/docs/Mozilla/Add-ons/WebExtensions/Native_messaging)
- [Native manifests](/en-US/docs/Mozilla/Add-ons/WebExtensions/Native_manifests)
- [User actions](/en-US/docs/Mozilla/Add-ons/WebExtensions/User_actions)
- [Differences between API implementations](/en-US/docs/Mozilla/Add-ons/WebExtensions/Differences_between_API_implementations)
- [Chrome incompatibilities](/en-US/docs/Mozilla/Add-ons/WebExtensions/Chrome_incompatibilities)

## User interface

Discover all the [user interface](/en-US/docs/Mozilla/Add-ons/WebExtensions/user_interface) components you can use in your extensions, with coding examples and tips.

## How to

A range of tutorials to get you started on specific aspects of extension development.

- [Intercept HTTP requests](/en-US/docs/Mozilla/Add-ons/WebExtensions/Intercept_HTTP_requests)
- [Modify a web page](/en-US/docs/Mozilla/Add-ons/WebExtensions/Modify_a_web_page)
- [Safely insert external content into a page](/en-US/docs/Mozilla/Add-ons/WebExtensions/Safely_inserting_external_content_into_a_page)
- [Share objects with page scripts](/en-US/docs/Mozilla/Add-ons/WebExtensions/Sharing_objects_with_page_scripts)
- [Add a button to the toolbar](/en-US/docs/Mozilla/Add-ons/WebExtensions/Add_a_button_to_the_toolbar)
- [Implement a settings page](/en-US/docs/Mozilla/Add-ons/WebExtensions/Implement_a_settings_page)
- [Work with the Tabs API](/en-US/docs/Mozilla/Add-ons/WebExtensions/Working_with_the_Tabs_API)
- [Work with the Bookmarks API](/en-US/docs/Mozilla/Add-ons/WebExtensions/Work_with_the_Bookmarks_API)
- [Work with the Cookies API](/en-US/docs/Mozilla/Add-ons/WebExtensions/Work_with_the_Cookies_API)
- [Work with contextual identities](/en-US/docs/Mozilla/Add-ons/WebExtensions/Work_with_contextual_identities)
- [Interact with the clipboard](/en-US/docs/Mozilla/Add-ons/WebExtensions/Interact_with_the_clipboard)
- [Extend the developer tools](/en-US/docs/Mozilla/Add-ons/WebExtensions/Extending_the_developer_tools)
- [Build a cross-browser extension](/en-US/docs/Mozilla/Add-ons/WebExtensions/Build_a_cross_browser_extension)

## Firefox workflow

When you are ready to create your extension for Firefox or port your Chrome extension, head over to [Extension Workshop](https://extensionworkshop.com/). It has details on:

- The Firefox workflow, such as [temporarily installing extensions during development](https://extensionworkshop.com/documentation/develop/temporary-installation-in-firefox/), [debugging](https://extensionworkshop.com/documentation/develop/debugging/), [request the right permissions](https://extensionworkshop.com/documentation/develop/request-the-right-permissions/), and more.
- The [web-ext](https://extensionworkshop.com/documentation/develop/getting-started-with-web-ext/) developer tool.
- [Porting a Google Chrome extension](https://extensionworkshop.com/documentation/develop/porting-a-google-chrome-extension/), [differences between desktop and Android](https://extensionworkshop.com/documentation/develop/differences-between-desktop-and-android-extensions/), and more.
- [Publishing and distribution overview](https://extensionworkshop.com/documentation/publish/), [promoting your extension](https://extensionworkshop.com/documentation/publish/promoting-your-extension/), the [extension lifecycle best practices](https://extensionworkshop.com/documentation/manage/), and more.

## Reference

### JavaScript APIs

Get comprehensive details about the methods, properties, types, and events for all the [JavaScript APIs](/en-US/docs/Mozilla/Add-ons/WebExtensions/API). There is also detailed information about the compatibility of each API with the major browsers. Most reference pages also include coding examples and links to the extension examples that use the API.

### Manifest keys

Get full details about the [manifest keys](/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json), including all their properties and settings.
