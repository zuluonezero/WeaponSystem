# WeaponSystem
WeaponSystem



    the character wields 3 weapons
    the character can check which weapons are currently available
    the character can invoke any of the weapons that are currently available
    each weapon becomes unavailable for a configured time after use
    the 3 weapons
        a weapon that deals immediate damage to the first character in a straight line from a point
        a weapon that deals damage at the end of each period for a window of time to any characters within a circle
        a weapon that deals damage at the start of each period for a window of time to a specific character


Set Up.

Player and Player_A are functionally the same.

Player is the most basic implementation (and will demonstrate first).

Player_A is a more advanced refacturing that decouples the relationship between the weapons and the weapon check components.

Fire 1 will do immediate damage to cube1 directly in front of the Player (and recharches in two seconds).
Fire 2 will damage all cubes in a 3 unit radius at the end ofa one second "round" for four seconds (and takes 5 seconds to recharge).
Fire 3 targets the BossCube directly and does damage at the start of each interval "round" for 20 seconds (recharge time is 10).

All events log to the Console to report hit/miss damage dealt and to whome the damage was inflicted.

A Weapons Check will report to the console what weapons are currently available.
