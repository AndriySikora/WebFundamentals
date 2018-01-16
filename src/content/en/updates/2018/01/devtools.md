project_path: /web/_project.yaml
book_path: /web/updates/_book.yaml
description: TODO

{# wf_updated_on: 2018-01-16 #}
{# wf_published_on: 2018-01-16 #}
{# wf_tags: chrome65,devtools,devtools-whatsnew #}
{# wf_featured_image: /web/updates/images/generic/chrome-devtools.png #}
{# wf_featured_snippet: TODO #}
{# wf_blink_components: Platform>DevTools #}

{% include "web/tools/chrome-devtools/_shared/styles.html" %}

# What's New In DevTools (Chrome 65) {: .page-title }

{% include "web/_shared/contributors/kaycebasques.html" %}

Note: The video version of these release notes will be published around
early-March 2018.

New features coming to DevTools in Chrome 65 include:

* Network overrides
* Color contrast line
* New audits
* Puppeteer 1.0
* Multiple Performance recordings
* Code stepping with workers
* New "Step Into" behavior

Note: Check what version of Chrome you're running at `chrome://version`. If you're running
an earlier version, these features won't exist. If you're running a later version, these features
may have changed. Chrome auto-updates to a new major version about every 6 weeks.

## Network overrides {: #overrides }

## Contrast ratio in the Color Picker {: #contrast-ratio }

The [Color Picker][CP] now shows you the contrast ratio of text elements. Increasing the
contrast ratio of text elements makes your site more accessible to users with low-vision
impairments or color deficiencies. See [Color and contrast][contrast] to learn more.

<figure>
  <img src="/web/updates/images/2018/01/contrast-ratio-collapsed.png"
       alt="Inspecting the contrast ratio of the highlighted H1 element."/>
  <figcaption>
    <b>Figure X</b>. Inspecting the contrast ratio of the highlighted <code>h1</code> element
  </figcaption>
</figure>

Click **Show More** ![Show More][SM]{:.cdt-inl} to expand the **Contrast Ratio** section.

<figure>
  <img src="/web/updates/images/2018/01/contrast-ratio-expanded.png"
       alt="The expanded Contrast Ratio section."/>
  <figcaption>
    <b>Figure X</b>. The expanded <b>Contrast Ratio</b> section
  </figcaption>
</figure>

Note: The **Audits** panel has an automated accessibility audit for ensuring that
each text element on a page has a sufficient contrast ratio. See [Run Lighthouse in Chrome
DevTools][audit] to get started with the **Audits** panel.

[CP]: /web/tools/chrome-devtools/css/reference#color-picker
[contrast]: /web/fundamentals/accessibility/accessible-styles#color_and_contrast
[SM]: /web/updates/images/2018/01/show-more.png
[audit]: /web/tools/lighthouse/#devtools

## New audits {: #audits }

Chrome 65 ships with new performance audits:

* JavaScript boot-up time is high
* Uses inefficient cache policy on static assets
* Avoids page redirects

And a whole new category of SEO audits:

* Document doesn't use legible font sizes
* Has a `<meta name="viewport">` tag with `width` or `initial-scale`
* Document has a `<title>` element
* Document has a `meta` description
* Page has successful HTTP status code
* Links have descriptive text
* Page isn't blocked from indexing
* Document has a valid `hreflang`

Other updates include:

* New, manual accessibility audits
* Updates to the WebP audit to make
* A rehaul of the accessibility score

Note: The **Audits** panel is powered by [Lighthouse][LH]. Chrome 64 runs Lighthouse version 2.5.
Chrome 65 runs Lighthouse version 2.7. So this section is simply a summary of the [Lighthouse
2.6 Updates][2.6] and [Lighthouse 2.7 Updates][2.7].

[LH]: /web/tools/lighthouse
[2.6]: /web/updates/2017/12/lighthouse
[2.7]: /web/updates/2018/01/lighthouse


## Feedback {: #feedback }

The best place to discuss any of the features or changes you see here is
the [google-chrome-developer-tools@googlegroups.com mailing list][ML]. You
can also tweet us at [@ChromeDevTools](https://twitter.com/chromedevtools) if
you're short on time. If you're sure that you've encountered a bug in
DevTools, please [open an issue](https://crbug.com/new).

[ML]: https://groups.google.com/forum/#!forum/google-chrome-developer-tools

## Previous release notes {: #links }

See the [devtools-whatsnew][tag] tag for links to all previous DevTools
release notes.

[tag]: /web/updates/tags/devtools-whatsnew
