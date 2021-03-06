# Diaspora

Implementation Home Page URL: https://diasporafoundation.org/

Source code repo URL(s) (optional):
* [x] 100% open source implementation

Programming Language(s): Ruby

Developer(s): [Diaspora Community](https://github.com/diaspora/diaspora/graphs/contributors)

Answers are:
* [x] Confirmed via websub.rocks (for applicable results)
* [ ] All results are self-reported

## Discovery

* The publisher produces URLs with the following content types:
  * [ ] HTML
  * [x] Atom
  * [ ] RSS
  * [ ] JSON
  * Other ________
* [ ] The publisher advertises the hub and self URLs in HTTP headers
* The publisher advertises the hub and self URLs in the body of the document for the following content types:
  * [ ] HTML in <link> tags in the HTML <head>
  * [ ] HTML in <link> tags in the body (currently not allowed, but the restriction of placing the <link> tags in the <head> is *at risk* so if an implementation requires advertising the URLs in the body this limitation may be dropped)
  * [x] Atom in <link> elements
  * [ ] RSS in <atom:link> elements
* [ ] The publisher advertises the hub URL using the `.host-meta` well-known URI (currently *at risk*)

## Distribution

* [x] The publisher notifies the hub when a topic has been updated. (This is required, although the implementation details are not specified, in order to allow flexibility in how hubs are implemented. e.g. a hub integrated with the publishing software does not need a standardized notification mechanism.)

If your publisher uses an external hub, please describe how the publisher notifies the hub of new content:

* [ ] The publisher sends a POST request to the hub with `hub.mode=publish&hub.topic=_______`
* [x] Other: POST request to the hub with `hub.mode=publish&hub.url=_______`

## Notes

* This is not reported by the diaspora team, but by a third party on their behalf of current released code.
