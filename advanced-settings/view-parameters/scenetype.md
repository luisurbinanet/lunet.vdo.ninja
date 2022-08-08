---
description: Shows only the last added video to a scene
---

# \&scenetype

Viewer-Side Option! ([`&view`](view.md), [`&scene`](scene.md))

## Aliases

* `&type`

## Options

| Value | Description                                                                                                                                               |
| ----- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1     | just shows the last guest that was added in the scene, but doesn't mute the previous guests                                                               |
| 2     | just shows the last guest that was added in the scene                                                                                                     |
| 3     | the general idea is it will only show the video that is in a particular ordered position (default, position = 1), rather than all the videos in the scene |

## Details

You can change the behaviour of scenes a bit with this parameter.\
\
Scene type can be set to 1 or 2, which overrides the default scene state.\
\
Scene state of 1 and 2 will only show the last video added to a group scene. Scene type 2 will mute the other videos, while scene type of 1 will not mute previously added videos.\
\
added `&scenetype=3` to beta. Usage is like this: `&scene&room=asdfasdfsdfsf3232&scenetype=3&order=1` , where [`&order=N`](../../source-settings/order.md) is optional. This feature isn't set in stone yet, but the general idea is it will only show the video that is in a particular ordered position (default, position = 1), rather than all the videos in the scene. When someone leaves, the spots are recalculated. The order that the positions are based on is calculated via alphanumeric sorting of connection IDs, though I wish to improve this to be probably sync with the director's order. Anyways, this feature was a result of a user request.

This URL parameter option is a bit of a hack currently and may be replaced in the future.

This parameter is added to scene view links.

## Related

{% content-ref url="scene.md" %}
[scene.md](scene.md)
{% endcontent-ref %}