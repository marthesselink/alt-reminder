# Alt Reminder :rotating_light:
Get a reminder when you forget the alt attribute to enhance digital accessibility,
for everyone.

## Why?
An alt-text is a description of an image that’s shown to people who, for some reason, can’t see the image. This can be because of data saving or because of having little or no vision.

Mostly these people use something called a screen reader to navigate the web. A screen reader can't display the image, instead it reads the alt text. So when you're reading an article. It will read:

> Image: 'Five people in line at a supermarket.' - Supermarkets start giving away presents during the summer.

Now this is helpful for someone who can't see the image. Alt texts that aren't helpful are:
> cropped_img224_300px.png

> \<Article title>

> Credits: John Ling

## When not to use an alt text
**Important note: never remove the alt-attribute, you are allowed to set it to an empty string, that is: alt=””.**

1. Repeated images, like profile pictures in a timeline.
2. Icons with a textlabel. It will read:
 > Image:"Facebook" - Facebook

 > Image:"Menu" - Menu
3. Image in a link. It will distract the reader and the image will probably be present on the linked page.
4. Decorative Image. (Preferably place these as a background image.)

### More info
[Axess Lab article: Alt-texts: The Ultimate Guide](https://axesslab.com/alt-texts/)


## Install
```sh
bower install marthesselink/alt-reminder --save-dev
```

Or if you want to get reminded on the production site too:

```sh
bower install marthesselink/alt-reminder --save
```


## Usage

```scss
@include alt-reminder();
```

Apply the mixin to the body

### API
```scss
@include alt-reminder((
  'border-width': 5px,
  'error-color': #cc0000,
));
```

#### Border width
Width of the error border.

#### Error color
The color of ther error border.
