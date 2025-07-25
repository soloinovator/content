---
title: Updating extensions for Firefox 7
slug: Mozilla/Firefox/Releases/7/Updating_extensions
page-type: guide
sidebar: firefox
---

This article offers advice for add-on developers that want to update their extensions to work in Firefox 7. Fortunately, most of the changes are relatively minor in this release, and few add-ons should need significant changes to work in Firefox 7.

> [!NOTE]
> For a complete list of developer-related changes in Firefox 7, see [Firefox 7 for developers](/en-US/docs/Mozilla/Firefox/Releases/7).

As always, you will need to [recompile any binary components](https://web.archive.org/web/20210119071646/https://developer.mozilla.org/en-US/docs/Mozilla/Developer_guide/Interface_Compatibility#binary_interfaces) to make them compatible with Firefox 7.

## XPCOM changes affecting compatibility

Most of the changes in this release are XPCOM interface removals, or removals of specific, obsolete APIs from interfaces.

### Removed interfaces

The following interfaces are the ones that were removed that will most likely impact extension developers:

- `nsIDOM3Node`
- `nsIDOM3TypeInfo`
- `schemaTypeInfo`
- `nsIDOMNSDocument`
- `nsIDOMDocumentStyle`

You can get a complete list of the removed interfaces in the [Removed interfaces](/en-US/docs/Mozilla/Firefox/Releases/7#removed_interfaces) section of [Firefox 7 for developers](/en-US/docs/Mozilla/Firefox/Releases/7).

### Changed methods

A few interfaces have methods that have been changed:

- `nsINavHistoryObserver` and `nsINavBookmarkObserver`
  - : These have been changed to support Firefox Sync better by adding a new GUID parameter to several of their methods. JavaScript-based code shouldn't require any changes, since this is just the addition of a new, optional, parameter. However, binary components will need to be updated to take the new parameter into account.
- `nsIDOMFile`
  - : A number of non-standard methods have been removed from this interface. This affects the {{ domxref("File") }} object's `File.getDataAsUrl()` and `File.getAsBinary()` methods. However, this functionality can now be found in the standard {{ domxref("FileReader") }} object.

## Other changes of note

These changes won't affect compatibility (we weren't kidding when we said there weren't many changes that do in this release), but do add capabilities that are easy to take advantage of that might be of special use to you.

### Unloading JavaScript code modules

The new `Components.utils.unload()` method lets you unload JavaScript code modules previously loaded by calling `Components.utils.load()`. This can be particularly handy with restartless (bootstrapped) extensions, so that you can unload an old version of a code module when a new version of your add-on is installed.

### Inline preferences

You can now have [preference options inline](https://web.archive.org/web/20210417084958/https://developer.mozilla.org/en-US/docs/Archive/Add-ons/Inline_Options) in the Add-on Manager window, which lets users configure your add-on without having to open a separate preference dialog box. There are limits to what types of configuration controls can be provided, but this is still very helpful — plus it works for [restartless (bootstrapped) extensions](https://web.archive.org/web/20210519000929/https://developer.mozilla.org/en-US/docs/Archive/Add-ons/Bootstrapped_extensions).

## See also

- [Firefox 7 for developers](/en-US/docs/Mozilla/Firefox/Releases/7)
- [Add-ons Blog: Firefox 7 add-on compatibility](https://blog.mozilla.org/addons/2011/07/19/firefox-7-compat-looking-to-8/)
- [XPCOM changes in Gecko 2.0](https://web.archive.org/web/20210514105748/https://developer.mozilla.org/en-US/docs/Mozilla/Tech/XPCOM/Guide/Changes_in_Gecko_2.0)
