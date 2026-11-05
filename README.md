# Typography

*Version from 2026-11-05 for UrqW 2.0.*

A plugin for [UrqW](https://github.com/urqw/UrqW) that automatically improves typography.

All text displayed on the screen using the `pln`/`println`, `p`/`print`, and `btn` operators is preprocessed to perform various typographic transformations, such as replacing basic typewritten characters with proper hyphens, dashes, quotation marks, and more.
Character replacements are performed in accordance with specified national rules and traditions (approximately 10 languages ??are supported).
For a full list of the transformations performed, see the plugin usage example.

Usage Features:

* Connect the plugin to the game. It will start working automatically. In most simple cases, the default configuration will be sufficient.
* You can explicitly set the language of the typographic tradition using the `urqw_typography_lang` variable. If it is not set or has an empty value, the plugin will use the language from the `urqw_game_lang` variable.
* If you need to enable or disable automatic typographic transformations, you can do so using the `urqw_typography_off` variable: value that is equivalent to `true` in a Boolean context disables automatic text transformations.
* If you need to process specific text, the `Typography()` URQL function can be called. It takes the text (required) as its first parameter, and the language code (optional) as its second.

For more details, see the plugin usage example.

The plugin and an example of its use can be found in the urqw directory. A demo of the plugin can be viewed at <https://urqw.github.io/UrqW#typography>

For other UrqW plugins, see the [common repository](https://github.com/urqw/plugins).

Be careful, though: not all UrqW plugins can be easily combined.
