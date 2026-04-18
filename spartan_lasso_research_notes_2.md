# Spartan Lasso Research Notes

Generated from uploaded `lasso_animations.zip`.

## Inventory
- Total files: 75
- getup_transitions: 8
- ragdoll: 1
- inventory_equip: 6
- grapple: 4
- melee: 1
- motion_tasks_mrf: 12
- horseback: 32
- introflow: 4
- meta: 2
- expression_yed: 2
- other: 3

## Key findings
- Rockstar splits lasso behavior across four layers: data/meta, rope physics tuning, animation dictionaries, and motion-relation task graphs.
- `lassodata.meta` maps entity models to lasso behavior flags like `CanBeLassoed`, `CanBeLassoedWhenDead`, `CanPullOverPlayer`, `ShouldFleeOnAttach`, and `ShouldAttackOnAttach`.
- `lassodata.meta` also contains attachment presets with named target bones and weighted attach points such as `ID_SKEL_NECK2`, `ID_CP_F_NECKLASSO`, `ID_CP_R_NECKLASSO`, and `ID_CP_B_NECKLASSO`.
- `lassotuning.meta` exposes rope solver and feel values: rope type, solver iteration counts, stretch/compression weights, gravity factors, damping, handle radius, bend angle limits, loop-drive-to-animation factors, and attachment speed/radius thresholds.
- Animation coverage includes on-foot, mounted, inventory/equip, ragdoll, get-up transitions, melee/grapple states, and multiplayer introflow poses.
- Horseback lasso is especially rich: ready, swing, reel-in, drag, loosen, tighten, yank, pull-off, and many transition clips.
- `s_mp_lassoloop01x.yed.xml` looks like an expression/rig driver for the visible lasso loop model rather than a regular task animation.
- `.mrf` files appear to be motion relation/state graph resources that connect weapon and strafe locomotion to lasso-specific states.

## File groups
### getup_transitions
- `ai_getup@directional@transition@prone_to_knees@lasso@loosen_feet.ycd.xml`
- `ai_getup@directional@transition@prone_to_knees@lasso@loosen_hogtie.ycd.xml`
- `ai_getup@directional@transition@prone_to_knees@lasso@loosen_neck.ycd.xml`
- `ai_getup@directional@transition@prone_to_knees@lasso@loosen_waist.ycd.xml`
- `ai_getup@directional@transition@prone_to_seated@lasso@loosen_feet.ycd.xml`
- `ai_getup@directional@transition@prone_to_seated@lasso@loosen_hogtie.ycd.xml`
- `ai_getup@directional@transition@prone_to_seated@lasso@loosen_neck.ycd.xml`
- `ai_getup@directional@transition@prone_to_seated@lasso@loosen_waist.ycd.xml`

### ragdoll
- `ai_ragdoll@lasso.ycd.xml`

### inventory_equip
- `mech_inventory@equip@fallback@base@lasso.ycd.xml`
- `mech_inventory@equip@fallback@base@unarmed@satchel@lasso.ycd.xml`
- `mech_inventory@equip@fallback@base@unarmed@satchel@lasso_gesture.ycd.xml`
- `mech_inventory@equip@fallback@crouch@unarmed@satchel@lasso.ycd.xml`
- `mech_inventory@equip@fallback@first_person@unarmed@satchel@lasso_gesture.ycd.xml`
- `mech_inventory@equip@vehicle@shared@seated@base@unarmed@satchel@lasso_gesture.ycd.xml`

### grapple
- `mech_grapple@lasso@_male@_ambient@_healthy@mounted@_streamed.ycd.xml`
- `mech_grapple@lasso@_male@_ambient@_healthy@mounted@intimidation@on_ass@_base.ycd.xml`
- `mech_grapple@lasso@_male@_ambient@_healthy@mounted@intimidation@on_knees@_base.ycd.xml`
- `mega_mech_grapple@lasso@male@mounted.ycd.xml`

### melee
- `mech_melee@lasso@_male@_ambient@_healthy@_noncombat.ycd.xml`

### motion_tasks_mrf
- `tasklasso.mrf`
- `tasklassofallover.mrf`
- `taskmotionstrafe_idle_lasso.mrf`
- `taskmotionstrafe_moving_lasso.mrf`
- `taskmotionstrafe_startmoving_lasso.mrf`
- `taskmotionstrafe_stopmoving_lasso.mrf`
- `taskmotionweaponaiminglasso.mrf`
- `taskmotionweaponcoillasso.mrf`
- `taskmotionweaponcoillassohorseback.mrf`
- `taskmotionweaponfirereleaselasso.mrf`
- `taskmotionweaponintrolasso.mrf`
- `taskmotionweaponthrowlasso.mrf`

### horseback
- `veh_horseback@aim@front@special@lasso@base@loco.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@pull@loosen.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@pull@tighten_rope.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@pull@yank.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@pull_off.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@ready.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@reelin.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@reelin_drag.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@reelin_empty.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@reelin_empty_quick.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@reelin_heavy.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@reelin_lead.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@reelin_pull.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@release_wait.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@swing.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@ready_rear_turn.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@ready_to_swing.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@reelin_drag_rear_turn.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@reelin_drag_to_reelin_heavy.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@reelin_drag_to_reelin_lead.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@reelin_heavy_rear_turn.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@reelin_heavy_to_reelin.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@reelin_heavy_to_reelin_drag.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@reelin_lead_rear_turn.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@reelin_lead_to_reelin.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@reelin_lead_to_reelin_drag.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@reelin_rear_turn.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@reelin_to_reelin_heavy.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@reelin_to_reelin_lead.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@release_wait_rear_turn.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@swing_rear_turn.ycd.xml`
- `veh_horseback@aim@front@special@lasso@base@transitions@swing_to_ready.ycd.xml`

### introflow
- `script_mp@introflow@soloonfoot@lasso.ycd.xml`
- `script_mp@introflow@soloonhorse@lasso.ycd.xml`
- `script_mp@introflow@teamonfoot@lassos.ycd.xml`
- `script_mp@introflow@teamonhorse@lassos.ycd.xml`

### meta
- `lassodata.meta`
- `lassotuning.meta`

### expression_yed
- `cp_lasso.yed.xml`
- `s_mp_lassoloop01x.yed.xml`

### other
- `mech_jump@arms@lasso.ycd.xml`
- `mega_mech_strafe@generic@lasso.ycd.xml`
- `mega_mech_weapons_special@lasso.ycd.xml`

## Practical engineering takeaways
- For believable lasso control, do not treat it as only a prop and one animation. The game uses rope tuning, attach-point rules, motion task graphs, and many contextual anim dictionaries together.
- For custom whip/rope systems, the best reusable parts are: attach point ideas from `lassodata.meta`, motion state naming from the `.mrf` set, and staged animation families from the horseback/on-foot dictionaries.
- A future parser should extract: dictionary name, clip names, inferred context tags (mounted/on-foot/getup/reelin/tighten/yank), and any bone/attachment references.