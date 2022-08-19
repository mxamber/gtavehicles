# gtavehicles
In `gtavehicles.json` I've compiled a (as yet incomplete) list of GTA Online's vehicles. The focus is not on stats, tuning or equipment, but  rather on dependencies: where is it bought, where is it stored, what other vehicles or properties does it require, and what does it unlock? A technology tree *sans* tree, basically.

## Template

A vehicle should have the following  data:

```
id {
  name        (string): in-game name
  maker       (string): manufacturer, if one exists
  price_trade    (int): discounted price if one exists
  price_full     (int): regular price
  storage     (string): what property it's stored in, or "none"
  type        (string): car/plane/helicopter/drone
  venue       (string): warstock/superautos/motorsport/elitas/docktease
  capacity       (int): incl. driver
  customizable  (bool): yes/no (only respray = no)
  weaponized    (bool): is or can be weaponized
  is_personal   (bool): can be stored in a personal garage?
  is_pegasus    (bool): can be ordered from pegasus?
  is_special    (bool): can be spawned via interaction menu
                        (services/special vehicles/ceo vehicles)
  enables   (string[]): vehicles or properties unlocked by this one
  depends   (string[]): vehicles or properties this vehicle requires (AND/OR)
                        (incl. ones required to customize the car, e.g. Avenger)
}
```

## Contributing

See something wrong? See missing vehicles? Open an issue or a pull request. Please explain what you want changed and why.
