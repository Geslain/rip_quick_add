# RIP Quick Add

Quickly create Google Calendar events from natural language.

![preview.gif](https://raw.githubusercontent.com/mtimkovich/rip_quick_add/main/preview.gif)

Quick Add was a Google Calendar feature that enabled creating calendar events from natural language text input. It was removed for no reason and [upset many people][support]. This is my attempt to carry on its legacy. It uses the [Chrono][chrono] library to extract time data from text.

## How it works

1. Takes a text input e.g. "Dinner friday 7pm"
2. Parses the input to find date info
3. Returns a Google Calendar URL for adding the event to your calendar.

Events can be created by either highlighting date information and selecting the extension in the context menu or by clicking the extension icon and entering event info into the text field.

## Usage

### Chrome Extension
Install the Chrome extension from [Chrome Web Store][webstore].

### Web App
Alternatively, I have a running implementation [on my website][max]. This is useful when you're on a device without Chrome extensions, like a phone.

#### Local
If you want to run the webapp locally:

```
yarn install
yarn start
```

## Documentation

The "API" this app is using is documented [here][docs].

# Author

Max Timkovich

[support]: https://support.google.com/calendar/thread/55538170/can-quick-add-be-reinstated?hl=en
[docs]: https://github.com/InteractionDesignFoundation/add-event-to-calendar-docs/blob/main/services/google.md#google
[max]: https://timkovi.ch/rip_quick_add
[chrono]: https://github.com/wanasit/chrono
[webstore]: https://chrome.google.com/webstore/detail/rip-quick-add/einookkhlkagdckkngcebldmicpilpmk
