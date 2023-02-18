# Mod Development Notes

## Ant Code Locations
* Ant unit configurations are located in the `UDATA.CPP` file.
* Ant animations are in the `UNIT.CPP` file.
* Ant Hill stuff is found in the `REINF.CPP` file.
* Ants are declared in the `DEFINES.H` file.
* Ants are also found in the `Rules.ini` file.
** Including the 3 ant types, along with the Queen ant being in the buildings section.
** This can only modify the units' attributes however, so deeper modification can't be done here.

## Important Code Locations
* Useful things to understand game logic are in the `TECHNO.CPP` file.

### `UDATA.CPP`
* Ant unit configurations are in this file
* Unit configurations are passed to a constructor

### `DEFINES.H`
* Game object states (or behaviours) are in `MissionType` on line 1010.
* Building animations are in `BStateType` on line 1047.
* Actions are defined in `ActionType` on line 1067.
* Factions are defined in `HousesType` in line 1171.
* Infantry units are defined in `InfantryType` on line 1561.
* Other land units (vehicles, hovercraft, etc.) are defined in `UnitType` on line 1612.
** Ant units are defined in `UnitType` -- I was thinking they should be in here anyways.
* Naval units are defined in `VesselType` on line 1672.
* Air units are defined in `AircraftType` on line 1709.
* Selected unit boxes are defined in `SelectEnum` on line 2528.
** Ants will probably take the bigger box defined by `SELECT_UNIT`.
* Different weapons are defined in `WeaponType` on line 2691.
* Armor types are defined in `ArmorType` on line 2758.
* Sounds are defined in `VocType` on line 3152.