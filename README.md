# OGDCH_HANDBOOK

> Anticloud offline package — upstream: opendata-swiss/ogdch-handbook @ `master`.

## What This Project Does

Home of the handbook of opendata.swiss: https://handbook.opendata.swiss/

## Upstream README

# Handbook for opendata.swiss

## About

This is the handbook for [opendata.swiss](https://opendata.swiss/).
It is published at https://handbook.opendata.swiss.

### Content and Target Group

The handbook is targeted towards data publishers and data users:

- data publishers get guidance on how to publish their data for themselves
  and on opendata.swiss
- data users find instructions on how to use the data via api and
  how to search for data on opendata.swiss

### Language Versions

It is currently available in the two languages German and French. German is its original
language and French is added as a translation. Some content is provided in English
language, which is currently not considered as a translation but rather as a fallback
for text, that does not come with language versions yet.

### History

This repo replaces the previous version of the handbook, which can be found here:
https://github.com/opendata-swiss/ogd-handbook-site

## Technical setup

The handbook is implemented with [Sphinx](https://www.sphinx-doc.org/en/master/),
Sphinx is a static site generator for documentations.
The source code is written in [reStructuredText](https://en.wikipedia.org/wiki/ReStructuredText).

The handbook is structured into:
- The **Source**: as reStructuredText
- The **Translations**: as string translations

The **Source** can be found at `source/content` with some pages such as the homepage `source/index.rst`
directly in the `source` directory. All source files have the ending `.rst` as they contain
reStructuredText.
Most source files are in German language, some are written in English.
No matter what language of these files are in: German or English: the `.rst` files are considered together as
the German/source version of the handbook.

The **Translations** can be found at `source/locale`. They contain text strings that have
been extracted from the **Source**. These text strings are stored along with translations in `.po` files.
If no translation is given in these files: the fallback is the original text in the **Source**.
The tool used for translations is
[sphinx-intl](https://www.sphinx-doc.org/en/master/usage/advanced/intl.html)

**Locales**: Currently there are two locales of the handbook:
- a German locale at `source/locale/de`: the translations there are left empty, so that the fallback, the **Source**
  is used
- a French locale at `source/locale/fr`: stores the translatable strings from the **Source** together with French
  translations for all German texts. English texts have not been translated.

## Local development

### Setup

The handbook can be downloaded and setup locally on your Computer.
First open a terminal window and clone the repo:

```commandline
git clone git@github.com:opendata-swiss/ogdch-handbook.git
cd ogdch-handbook
```

If you want to be able to build the handbook locally from its
**Source**, then you need to set up the virtual python3 environment and install the
requirements, as shown below:

```commandline
python3 -

## License

Upstream terms preserved in `THIRD_PARTY_LICENSES/`. Overlay licensed under Anticommons 0.1.0.

## Verification

Recompute the SHA3-256 of `BENCH.json` and compare to this package’s register. Any drift = invalid package.
