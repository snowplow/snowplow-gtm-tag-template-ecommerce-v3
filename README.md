# Snowplow v3 Ecommerce GTM Tag Template

[![early-release]][tracker-classification]
[![License][license-image]][license]
[![Release][release-image]][releases]

[Snowplow][snowplow] is a scalable open-source platform for rich, high quality, low-latency data collection. It is designed to collect high quality, complete behavioral data for enterprise business.

## Overview

This is a Google Tag Manager [custom tag template][gtm-custom-template] for implementing Ecommerce tracking using the [Snowplow JavaScript tracker v3][javascript-tracker] and its [Snowplow Ecommerce plugin][snowplow-ecommerce-plugin].

It has been designed to be used with the [Snowplow v3 Settings variable template][gtm-v3-settings-variable] and can be implemented along the [Snowplow v3 tag template][gtm-v3-tag].

## Quickstart

### Installing from the Google Tag Manager Gallery

_Coming soon!_

### Manual Installation

To manually install the tag template:

1. Download `template.tpl`
2. Create a new Tag template in the Templates section of your GTM container
3. Click the More Actions menu and select Import
4. Import `template.tpl` downloaded in Step 1
5. Click Save.

## Find out more

| Technical Docs                    |
|-----------------------------------|
| [![i1][techdocs-image]][techdocs] |
| [Technical Docs][techdocs]        |

## Maintainer Quickstart

Work on the template should be done in Google Tag Manager's native **template editor**. This is to ensure the template has access to all the latest features of the template editor, and to make sure it passes GTM's own validation when exporting the changes.

To **import** the template into Google Tag Manager:

1. In a Google Tag Manager **web** container, browse to **Templates** and click to create a new template.
2. From the template action menu, choose **Import**.
3. Locate the `template.tpl` file from this repo, and import it into the template editor.

Make the changes you wish. Make sure the unit tests pass (in the **Tests** tab of the editor). Update the tests if necessary.

Once you're done, follow these steps:

1. **Save** the template in the template editor.
2. From the action menu, choose **Export**.
3. Replace the `template.tpl` file in this repo with the exported file (make sure to keep `template.tpl` as its name).
4. **Commit** the changes to the `template.tpl` file and repeat if necessary.
5. Copy the last **commit hash**.
6. Edit `metadata.yaml` in the template folder, and add the hash with its `changeNotes` as the latest version.
7. Move the previous latest version into the list of `Older versions`.
8. Save changes to `metadata.yaml` and **commit** them using a **Prepare for x.y.z release** commit message.
9. Finally, push the changes to the repo (should include at least 2 commits as described above).

Once the tag is published in the GTM [community gallery][gtm-gallery] the template will be updated automatically within some time after the changes.

## Contributing

Feedback and contributions are welcome! If you have identified a bug, please log an issue on this repo. For all other feedback, discussion or questions please open a thread on our [discourse forum][discourse].

| Contributing                              |
|-------------------------------------------|
| [![i2][contributing-image]][contributing] |
| [Contributing][contributing]              |

## Copyright and license

Copyright (c) 2023 Snowplow Analytics Ltd.

Licensed under the **[Apache License, Version 2.0][license]** (the "License");
you may not use this software except in compliance with the License.

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

[tracker-classification]: https://docs.snowplow.io/docs/collecting-data/collecting-from-own-applications/tracker-maintenance-classification/
[early-release]: https://img.shields.io/static/v1?style=flat&label=Snowplow&message=Early%20Release&color=014477&labelColor=9ba0aa&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAAeFBMVEVMaXGXANeYANeXANZbAJmXANeUANSQAM+XANeMAMpaAJhZAJeZANiXANaXANaOAM2WANVnAKWXANZ9ALtmAKVaAJmXANZaAJlXAJZdAJxaAJlZAJdbAJlbAJmQAM+UANKZANhhAJ+EAL+BAL9oAKZnAKVjAKF1ALNBd8J1AAAAKHRSTlMAa1hWXyteBTQJIEwRgUh2JjJon21wcBgNfmc+JlOBQjwezWF2l5dXzkW3/wAAAHpJREFUeNokhQOCA1EAxTL85hi7dXv/E5YPCYBq5DeN4pcqV1XbtW/xTVMIMAZE0cBHEaZhBmIQwCFofeprPUHqjmD/+7peztd62dWQRkvrQayXkn01f/gWp2CrxfjY7rcZ5V7DEMDQgmEozFpZqLUYDsNwOqbnMLwPAJEwCopZxKttAAAAAElFTkSuQmCC

[license]: https://www.apache.org/licenses/LICENSE-2.0
[license-image]: https://img.shields.io/badge/license-Apache--2-blue.svg?style=flat

[releases]: https://github.com/snowplow/snowplow-gtm-tag-template-ecommerce-v3/releases
[release-image]: https://img.shields.io/github/v/release/snowplow/snowplow-gtm-tag-template-ecommerce-v3

[snowplow]: https://snowplow.io
[discourse]: https://discourse.snowplow.io

[gtm-v3-tag]: https://docs.snowplow.io/docs/collecting-data/collecting-from-own-applications/javascript-trackers/web-tracker/google-tag-manager-custom-template/tag-template-guide/
[gtm-v3-settings-variable]: https://docs.snowplow.io/docs/collecting-data/collecting-from-own-applications/javascript-trackers/web-tracker/google-tag-manager-custom-template/settings-variable-guide/
[javascript-tracker]: https://docs.snowplow.io/docs/collecting-data/collecting-from-own-applications/javascript-trackers/
[snowplow-ecommerce-plugin]: https://docs.snowplow.io/docs/collecting-data/collecting-from-own-applications/javascript-trackers/web-tracker/plugins/snowplow-ecommerce/

[techdocs]: https://docs.snowplow.io
[techdocs-image]: https://d3i6fms1cm1j0i.cloudfront.net/github/images/techdocs.png

[contributing-image]: https://d3i6fms1cm1j0i.cloudfront.net/github/images/contributing.png
[contributing]: CONTRIBUTING.md

[gtm-custom-template]: https://developers.google.com/tag-manager/templates
[gtm-gallery]: https://tagmanager.google.com/gallery
