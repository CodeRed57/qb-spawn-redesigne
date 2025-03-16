# qb-spawn
Spawn Selector for QB-Core Framework :eagle:

# License

    QBCore Framework
    Copyright (C) 2021 Joshua Eger

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <https://www.gnu.org/licenses/>


## Dependencies
- [qb-core](https://github.com/qbcore-framework/qb-core)
- [qb-houses](https://github.com/qbcore-framework/qb-houses) - Lets player select the house
- [qb-apartment](https://github.com/qbcore-framework/qb-apartment) - Lets player select the apartment
- [qb-garages](https://github.com/qbcore-framework/qb-garages) - For house garages

## Screenshots
![Image 1](https://r2.fivemanage.com/vMOkCnozwKRq1GH8rhuLB/image/Screenshot2025-03-16213421.png)
![Image 2](https://r2.fivemanage.com/vMOkCnozwKRq1GH8rhuLB/image/Screenshot2025-03-16213352.png)

## Features
- Ability to select spawn after selecting the character

## Installation
### Manual
- Download the script and put it in the `[qb]` directory.
- Add the following code to your server.cfg/resouces.cfg
```
ensure qb-core
ensure qb-spawn
ensure qb-apartments
ensure qb-garages
```

## Configuration
An example to add spawn option
```
QB.Spawns = {
    ["spawn1"] = { -- Needs to be unique
        coords = vector4(1.1, -1.1, 1.1, 180.0), -- Coords player will be spawned
        location = "spawn1", -- Needs to be unique
        label = "Spawn 1 Name", -- This is the label which will show up in selection menu.
        description = "lorem ipsum dolor sit amet", -- This is the description which will show up in selection menu.
        image = 'images/default.png', This is the image which will show up in selection menu.
    },
    ["spawn2"] = { -- Needs to be unique
        coords = vector4(1.1, -1.1, 1.1, 180.0), -- Coords player will be spawned
        location = "spawn2", -- Needs to be unique
        label = "Spawn 2 Name", -- This is the label which will show up in selection menu.
        description = "lorem ipsum dolor sit amet", -- This is the description which will show up in selection menu.
        image = 'images/default.png', This is the image which will show up in selection menu.
    },
}
```
