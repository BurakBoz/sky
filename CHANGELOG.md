# Changelog

All notable changes to `sky` will be documented in this file

## v3.1.0 - 2023-09-12

### stable version:

Since [tiptap editor](https://github.com/awcodes/filament-tiptap-editor) still in beta, I decided to make `MarkdownEditor` the default editor, if you want to use other one you can set it in the panel configuration.

#### ⚠️⚠️ the configuration for models has been changed to:

```php
->skyModels([
        'Faq' => \LaraZeus\Sky\Models\Faq::class,
        'Post' => \LaraZeus\Sky\Models\Post::class,
        'PostStatus' => \LaraZeus\Sky\Models\PostStatus::class,
        'Tag' => \LaraZeus\Sky\Models\Tag::class,
        'Library' => \LaraZeus\Sky\Models\Library::class,
    ])

```
#### What's Changed

- Add tiptap editor by @atmonshi in https://github.com/lara-zeus/sky/pull/131
- Update TipTapEditor.php by @atmonshi in https://github.com/lara-zeus/sky/pull/133
- refactor-editors by @atmonshi in https://github.com/lara-zeus/sky/pull/135
- Breadcrumbs and update SEO by @atmonshi in https://github.com/lara-zeus/sky/pull/141
- Update configuration.md by @atmonshi in https://github.com/lara-zeus/sky/pull/142
- remove config from `PublishCommand` by @atmonshi in https://github.com/lara-zeus/sky/pull/143
- improve queries by @atmonshi in https://github.com/lara-zeus/sky/pull/144
- fix duplicated breadcrumbs by @atmonshi in https://github.com/lara-zeus/sky/pull/145
- push filament styles when embedding a form by @atmonshi in https://github.com/lara-zeus/sky/pull/146
- update Render Nav Item class to include libraries items by @atmonshi in https://github.com/lara-zeus/sky/pull/148
- Update MarkdownEditor.php by @albertobenavides in https://github.com/lara-zeus/sky/pull/149
- refactor configuration model by @atmonshi in https://github.com/lara-zeus/sky/pull/151
- add RichEditor and update MarkdownEditor  by @atmonshi in https://github.com/lara-zeus/sky/pull/152

#### New Contributors

- @albertobenavides made their first contribution in https://github.com/lara-zeus/sky/pull/149

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.4.34...v3.1.0

## 2.4.34 - 2023-07-14

### What's Changed

- fix: show pages in the sidebar and no result for search by @atmonshi in https://github.com/lara-zeus/sky/pull/129
- add Content parser by @atmonshi in https://github.com/lara-zeus/sky/pull/118

adding the ability to parse the content, by default: `BoltParser` is avaliable.
lets you include or (embed) bolt form into any page with the syntax: `<bolt>formSlug</bolt>`
This will be parsed to a livewire component to display the full form.

### How to use:

Make sure to add this to your config:

```php
'parsers' => [
    \LaraZeus\Sky\Classes\BoltParser::class,
],


```
You can copy that class and create your own parser, too, then add it to the array, and Sky will loop them all.

```I
Of course, it will be visible only if you install Sky with Bolt :)

```
<img width="1165" alt="Screenshot 2023-07-14 at 6 26 23 PM" src="https://github.com/lara-zeus/sky/assets/1952412/5b62af0f-ac6b-46c7-ae29-af01975a9976">
### Remember to update your views.
**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.4.33...2.4.34

## 2.4.33 - 2023-07-12

### What's Changed

- Allow to skip highlighting of search terms by @thyseus in https://github.com/lara-zeus/sky/pull/125
- fix when library is empty by @atmonshi in https://github.com/lara-zeus/sky/pull/126
- update composer by @atmonshi in https://github.com/lara-zeus/sky/pull/127

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.4.32...2.4.33

## 2.4.32 - 2023-07-12

### What's Changed

- allow to upload multiple libraries and refactor the views by @atmonshi in https://github.com/lara-zeus/sky/pull/123
- update core by @atmonshi in https://github.com/lara-zeus/sky/pull/124

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.4.31...2.4.32

## 2.4.31 - 2023-07-04

### What's Changed

- Bump dependabot/fetch-metadata from 1.5.1 to 1.6.0 by @dependabot in https://github.com/lara-zeus/sky/pull/121
- update all dependecies by @atmonshi in https://github.com/lara-zeus/sky/pull/122

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.4.30...2.4.31

## 2.4.30 - 2023-07-02

### What's Changed

- allow to force delete and restore posts, and finally green phpstan by @atmonshi in https://github.com/lara-zeus/sky/pull/120

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.4.29...2.4.30

## 2.4.2 - 2023-04-24

### What's Changed

- add featured image by URL by @atmonshi in https://github.com/lara-zeus/sky/pull/72
- Default featured image from config by @atmonshi in https://github.com/lara-zeus/sky/pull/73
- Allow preview post for author by @atmonshi in https://github.com/lara-zeus/sky/pull/74
- update Zeus core by @atmonshi in https://github.com/lara-zeus/sky/pull/75

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.4.1...2.4.2

## 2.4.1 - 2023-04-10

### What's Changed

- Update configuration.md by @atmonshi in https://github.com/lara-zeus/sky/pull/70
- refactor getNavigationGroup by @atmonshi in https://github.com/lara-zeus/sky/pull/71

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.4.0...2.4.1

## 2.4.0 - 2023-04-10

### What's Changed

- Bump dependabot/fetch-metadata from 1.3.5 to 1.3.6 by @dependabot in https://github.com/lara-zeus/sky/pull/65
- Bump aglipanci/laravel-pint-action from 1.0.0 to 2.2.0 by @dependabot in https://github.com/lara-zeus/sky/pull/68
- Bump ramsey/composer-install from 1 to 2 by @dependabot in https://github.com/lara-zeus/sky/pull/63
- Added config for Navigation Group Label by @chahal26 in https://github.com/lara-zeus/sky/pull/66
- support laravel 10 by @atmonshi in https://github.com/lara-zeus/sky/pull/69

### New Contributors

- @chahal26 made their first contribution in https://github.com/lara-zeus/sky/pull/66

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.3.7...2.4.0

## 2.3.7 - 2022-11-12

### What's Changed

- small fixes in FAQ by @atmonshi in https://github.com/lara-zeus/sky/pull/62

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.3.6...2.3.7

## 2.3.6 - 2022-11-12

### What's Changed

- Add prose to faq by @leekaimun in https://github.com/lara-zeus/sky/pull/61

### New Contributors

- @leekaimun made their first contribution in https://github.com/lara-zeus/sky/pull/61

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.3.5...2.3.6

## 2.3.5 - 2022-11-11

### What's Changed

- Add prose classes by @atmonshi in https://github.com/lara-zeus/sky/pull/60

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.3.4...2.3.5

## 2.3.4 - 2022-11-08

### What's Changed

- Bump dependabot/fetch-metadata from 1.3.4 to 1.3.5 by @dependabot in https://github.com/lara-zeus/sky/pull/58
- add unique() constraint to slug fields by @thyseus in https://github.com/lara-zeus/sky/pull/57
- ensure only posts with status 'publish' are being shown in public by @thyseus in https://github.com/lara-zeus/sky/pull/56

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.3.3...2.3.4

## 2.3.3 - 2022-10-28

### What's Changed

- s/$getRecord/$getRecord() by @thyseus in https://github.com/lara-zeus/sky/pull/54

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.3.2...2.3.3

## 2.3.2 - 2022-10-04

### What's Changed

- Bump dependabot/fetch-metadata from 1.3.3 to 1.3.4 by @dependabot in https://github.com/lara-zeus/sky/pull/51
- PostScope: also search in 'slug' column by @thyseus in https://github.com/lara-zeus/sky/pull/52

### New Contributors

- @dependabot made their first contribution in https://github.com/lara-zeus/sky/pull/51

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.3.1...2.3.2

## 2.3.1 - 2022-09-18

### What's Changed

- improve SEO by @atmonshi in https://github.com/lara-zeus/sky/pull/50

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.3.0...2.3.1

## 2.3.0 - 2022-09-17

### What's Changed

- improve skeleton and add tests and dark mode
- separate the CSS for frontend and filament
- update .github workflows
- add phpstan and pint

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.2.6...2.3.0

## 2.2.6 - 2022-09-16

### What's Changed

- restore the post factory by @atmonshi in https://github.com/lara-zeus/sky/pull/48

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.2.5...2.2.6

## 2.2.5 - 2022-09-15

### What's Changed

- remove SEO from the service provider by @atmonshi in https://github.com/lara-zeus/sky/pull/41
- remove Factories by @thyseus in https://github.com/lara-zeus/sky/pull/42
- add route name slug by @thyseus in https://github.com/lara-zeus/sky/pull/44
- check for status on posts and pages by @atmonshi in https://github.com/lara-zeus/sky/pull/47

also checkout our roadmap: #46

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.2.4...2.2.5

## 2.2.4 - 2022-09-06

### What's Changed

- update core to fix lang switcher by @atmonshi in https://github.com/lara-zeus/sky/pull/40

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.2.3...2.2.4

## 2.2.3 - 2022-09-05

### What's Changed

- introduce the ability to filter posts by category by @thyseus in https://github.com/lara-zeus/sky/pull/35
- add Scopes for search by @atmonshi in https://github.com/lara-zeus/sky/pull/36
- update responsive design by @atmonshi in https://github.com/lara-zeus/sky/pull/38

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.2.2...2.2.3

## 2.2.2 - 2022-08-31

### What's Changed

- Apply fixes from StyleCI by @atmonshi in https://github.com/lara-zeus/sky/pull/34
- remove RouteKeyName slug by @atmonshi in https://github.com/lara-zeus/sky/pull/33

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.2.1...2.2.2

## 2.2.1 - 2022-08-24

### What's Changed

- abort if tag not exist by @atmonshi in https://github.com/lara-zeus/sky/pull/31
- update composer and assets by @atmonshi in https://github.com/lara-zeus/sky/pull/32

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.2.0...2.2.1

## 2.1.7 - 2022-08-15

### What's Changed

- French Translation by @nicolasbaud in https://github.com/lara-zeus/sky/pull/27
- refactor SEO and remove it form SkyServiceProvider by @atmonshi in https://github.com/lara-zeus/sky/pull/28

### New Contributors

- @nicolasbaud made their first contribution in https://github.com/lara-zeus/sky/pull/27

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.1.6...2.1.7

## 2.1.6 - 2022-07-10

### What's Changed

- Faq translation by @atmonshi in https://github.com/lara-zeus/sky/pull/25
- improvements by @atmonshi in https://github.com/lara-zeus/sky/pull/26

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.1.5...2.1.6

## 2.1.5 - 2022-07-05

### What's Changed

- introduce full-text search by @thyseus in https://github.com/lara-zeus/sky/pull/23

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.1.4...2.1.5

## 2.1.3 - 2022-06-21

update core version

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.1.2...2.1.3

## 2.1.2 - 2022-06-11

### What's Changed

- change translatable column types by @atmonshi in https://github.com/lara-zeus/sky/pull/21

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.1.1...2.1.2

## 2.1.1 - 2022-06-11

### What's Changed

- change namespace for Translatable by @atmonshi in https://github.com/lara-zeus/sky/pull/20

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.1.0...2.1.1

## 2.1.0 - 2022-06-11

### What's Changed

- add trans by @atmonshi in https://github.com/lara-zeus/sky/pull/14
- s/auther/author by @thyseus in https://github.com/lara-zeus/sky/pull/13
- introduce the ability to write posts and pages in different languages by @thyseus in https://github.com/lara-zeus/sky/pull/12
- introducing Addons: Faq by @atmonshi in https://github.com/lara-zeus/sky/pull/15

### New Contributors

- @thyseus made their first contribution in https://github.com/lara-zeus/sky/pull/13

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.0.5...2.1.0

## 2.0.5 - 2022-04-22

## What's Changed

- Apply fixes from StyleCI by @atmonshi in https://github.com/lara-zeus/sky/pull/11
- small fixes by @atmonshi in https://github.com/lara-zeus/sky/pull/10

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.0.4...2.0.5

## 2.0.4 - 2022-04-22

## What's Changed

- add missing validation by @atmonshi in https://github.com/lara-zeus/sky/pull/9

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.0.3...2.0.4

## 2.0.3 - 2022-04-21

## What's Changed

- fix preview links by @atmonshi in https://github.com/lara-zeus/sky/pull/5
- Apply fixes from StyleCI by @atmonshi in https://github.com/lara-zeus/sky/pull/6
- Configure prefix by @atmonshi in https://github.com/lara-zeus/sky/pull/7
- add some actions by @atmonshi in https://github.com/lara-zeus/sky/pull/8

**Full Changelog**: https://github.com/lara-zeus/sky/compare/2.0.2...2.0.3

## 2.0.0 - 2022-04-19

- the first stable release, and happy birthday to me :)
