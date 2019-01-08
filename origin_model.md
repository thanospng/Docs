# Origin model

## What's origin?
Origin is the tuple consisting of the scheme/protocol(eg. HTTP), the hostname(eg. www.google.com) and the port. In essence, origin defines a specific computer, application and protocol. If any of the three elements is different between two origins, the origins are different.

## Why is important?
Browser's use the origin model to keep each website's data secure and unreachable from other websites. This is called same-origin policy. Depending on the type of request, it may not be possible to retrieve a resource from a different origin, or even if they are retrieved, browsers may disallow what you can do with them. An example is images from a third origin that are not allowed to be used in canvas without explicitly asking them to do so.
