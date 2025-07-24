# ZMK `base-layer` behavior

This behavior (`&base`) allows to select a base layer and associate it to the current endpoint/profile.
When switching between endpoint/profiles the base layer is restored to the last one selected while on that endpoint/profile.

## Configuration

The configuration for this behavior consists of a single optional `base-layer` property
listing which layers are considered base layers.
When selecting or restoring a base layer, the behavior will disable the listed base layers before enabling the new one.
If the `base-layers` property is not set the behavior will act like `&to` and disable all layers except the new one.
