---
layout: analytics
title: Audigent
description: Audigent Analytics Adapter
modulecode: hadronAnalytics
gdpr_supported: true
usp_supported: true
prebid_member: true
gvl_id: 561
enable_download: false
---

#### Use

The Audigent analytics adapter can be used by all clients after approval. For more information, 
please visit <a href="https://audigent.com">https://audigent.com</a> or contact our Prebid integration team at prebid@audigent.com.

The Audigent privacy policy is at [https://audigent.com/privacypolicy/](https://audigent.com/privacypolicy/).

#### Analytics Options

{: .table .table-bordered .table-striped }
| Parameter | Scope | Type | Description | Example |
| --- | --- | --- | --- | --- |
| provider | Required | String | The name of this module: `hadronAnalytics` | `hadronAnalytics` |
| options.publisherID | Required | Number | Audigent's PublisherID | `1234` |
| options.eventsToTrack | Required | Array of strings | Filters the set of tracked events | `['auctionEnd','bidWon']` |


### Example Configuration

```javascript
pbjs.enableAnalytics({
    provider: 'hadronAnalytics',
    options: {
        partnerId: 1234,    // change to the Partner Number you received from Audigent
        eventsToTrack: ['auctionEnd', 'auctionInit']
    }
});
```
