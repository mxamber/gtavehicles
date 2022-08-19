# gtavehicles
In `gtavehicles.json` I've compiled a (as yet incomplete) list of GTA Online's vehicles. The focus is not on stats, tuning or equipment, but  rather on dependencies: where is it bought, where is it stored, what other vehicles or properties does it require, and what does it unlock? A technology tree *sans* tree, basically.

## Template

A vehicle should have the following  data:

```
short name: internal identifier, need not match game files. is object name.
  name: in-game name
  maker: manufacturer, if one exists
  price_trade: discounted price if one exists
  price_full: regular price
  storage: what property it's stored in, or "none"
  type: car/plane/helicopter/drone
  venue: warstock/superautos/motorsport/elitas/docktease
  capacity: incl. driver
  customizable: yes/no (only respray = no)
  weaponized: is or can be weaponized
  is_personal: can be stored in a personal garage?
  is_pegasus: can be ordered from pegasus?
  is_special: can be spawned via interaction menu (services/special vehicles/ceo vehicles)
  enables: an array of vehicles or properties unlocked by this one
  depends: an array of vehicles or properties this vehicle requires (AND/OR, incl. ones required to customize the car, e.g. Avenger or Terrorbyte)
```

## Contributing

See something wrong? See missing vehicles? Open an issue or a pull request. Please explain what you want changed and why.
