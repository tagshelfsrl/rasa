# TagShelf Changelog

## Version 1.7.4.2

### Features

- Added a persistent slot (like the `requested_slot`) called `reset_slot`. This slot is used to persist a current retry count inside a form for each user.

## Version 1.7.4.1

### Features

- Added a persistent slot (like the `requested_slot`) called `form_id`. This slot is used to persist a form tracking reference id so the action server can notify changes on the form state.
