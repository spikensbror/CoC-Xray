# Artifact Refine System

## Description

The artifact refine system basically places an artifact definition into one of
two states; refined and unrefined. Unrefined artifacts cannot be equipped by
the player.

A new indicator for the Artifact tooltip has been added above the efficiency
indicator that tells whether or not an Artifact is refined.

## Gamedata

### Texts

The system depends on the presence of the following strings:

* `ui_inv_af_refined`: "Refined"
* `ui_inv_af_refined_true`: "Yes"
* `ui_inv_af_refined_false`: "No"

### UI

* Note: Make sure that you define `ui_am_refined` in `gamedata\configs\ui\textures_descr\ui_actor_sleep_screen.xml` or change it to another existing icon texture.

#### af_params.xml

    <prop_line ...>
        ...
	</prop_line>
    <refined x="0" y="0" width="257" height="20">
        <caption x="0" y="0" width="257" height="20" complex_mode="0">
            <texture>ui_am_refined</texture>
            <text color="ui_3" font="letterica16" vert_align="c" x="22" y="0"/>
        </caption>
        <value x="140" y="0" width="30" height="20" magnitude="100">
            <text font="letterica16" vert_align="c"/>
        </value>
    </refined>
    <condition ...>
        ...
	</condition>

#### af_params_16.xml

    <prop_line ...>
        ...
	</prop_line>
    <refined x="0" y="0" width="214" height="20">
        <caption x="0" y="0" width="15" height="20" stretch="1">
            <texture>ui_am_refined</texture>
            <text color="ui_3" font="letterica16" vert_align="c" x="18" y="0"/>
        </caption>
        <value x="117" y="0" width="30" height="20" magnitude="100">
            <text font="letterica16" vert_align="c"/>
        </value>
    </refined>
    <condition ...>
        ...
	</condition>