# Spartan Lasso YCD Deep Findings

Opened and parsed all 59 `.ycd.xml` files in the uploaded lasso archive.

- Total YCD files: 59
- Total clip entries: 794
- Total animation slots: 317
- Bone/control references seen in YCD tags: CP_L_Forearm, SKEL_L_HAND, SKEL_NECK0, SKEL_R_HAND

## Highest-value files
- `mech_grapple@lasso@_male@_ambient@_healthy@mounted@_streamed.ycd.xml`: struggle loops, exits, victim/attacker mounted grapple, references `SKEL_L_HAND`, `SKEL_R_HAND`, `SKEL_NECK0`.
- `mech_grapple@lasso@_male@_ambient@_healthy@mounted@intimidation@on_ass@_base.ycd.xml`: enter clips with attacker/victim variants, references `CP_L_Forearm` and `SKEL_NECK0`.
- `mech_grapple@lasso@_male@_ambient@_healthy@mounted@intimidation@on_knees@_base.ycd.xml`: same intimidation family, on-knees variant, references `CP_L_Forearm` and `SKEL_NECK0`.
- `mech_melee@lasso@_male@_ambient@_healthy@_noncombat.ycd.xml`: hogtie takedowns, shove, kick, stomp, hand refs `SKEL_L_HAND`, `SKEL_R_HAND`.
- `mega_mech_grapple@lasso@male@mounted.ycd.xml`: large mounted grapple aggregator with many enter/transition/tackle clips and hand/neck refs.

## Horseback family highlights
- ready, swing, release_wait, pull_off
- reelin, reelin_drag, reelin_empty, reelin_empty_quick, reelin_heavy, reelin_lead, reelin_pull
- pull loosen / tighten_rope / yank
- many rear-turn and state-to-state transitions

## Notes
- Not every YCD exposes readable item or prop names in plain XML tags. Some mostly expose clips/animations and internal signatures.
- The clearest readable bone/control references in this archive's YCD XMLs are `SKEL_L_HAND`, `SKEL_R_HAND`, `SKEL_NECK0`, and `CP_L_Forearm`.
- The deeper attachment model still lives mainly in `lassodata.meta`, while rope feel lives in `lassotuning.meta`.

## Full file-by-file index

### ai_getup@directional@transition@prone_to_knees@lasso@loosen_feet.ycd.xml
- Dict: `ai_getup@directional@transition@prone_to_knees@lasso@loosen_feet`
- Clips: 2
- Anims: 3
- Sample clips: pack:/front.clip, pack:/back.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### ai_getup@directional@transition@prone_to_knees@lasso@loosen_hogtie.ycd.xml
- Dict: `ai_getup@directional@transition@prone_to_knees@lasso@loosen_hogtie`
- Clips: 1
- Anims: 3
- Sample clips: pack:/front.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### ai_getup@directional@transition@prone_to_knees@lasso@loosen_neck.ycd.xml
- Dict: `ai_getup@directional@transition@prone_to_knees@lasso@loosen_neck`
- Clips: 2
- Anims: 3
- Sample clips: pack:/back.clip, pack:/front.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### ai_getup@directional@transition@prone_to_knees@lasso@loosen_waist.ycd.xml
- Dict: `ai_getup@directional@transition@prone_to_knees@lasso@loosen_waist`
- Clips: 2
- Anims: 3
- Sample clips: pack:/front.clip, pack:/back.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### ai_getup@directional@transition@prone_to_seated@lasso@loosen_feet.ycd.xml
- Dict: `ai_getup@directional@transition@prone_to_seated@lasso@loosen_feet`
- Clips: 2
- Anims: 3
- Sample clips: pack:/front.clip, pack:/back.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### ai_getup@directional@transition@prone_to_seated@lasso@loosen_hogtie.ycd.xml
- Dict: `ai_getup@directional@transition@prone_to_seated@lasso@loosen_hogtie`
- Clips: 1
- Anims: 3
- Sample clips: pack:/front.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### ai_getup@directional@transition@prone_to_seated@lasso@loosen_neck.ycd.xml
- Dict: `ai_getup@directional@transition@prone_to_seated@lasso@loosen_neck`
- Clips: 2
- Anims: 3
- Sample clips: pack:/front.clip, pack:/back.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### ai_getup@directional@transition@prone_to_seated@lasso@loosen_waist.ycd.xml
- Dict: `ai_getup@directional@transition@prone_to_seated@lasso@loosen_waist`
- Clips: 2
- Anims: 3
- Sample clips: pack:/front.clip, pack:/back.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### ai_ragdoll@lasso.ycd.xml
- Dict: `ai_ragdoll@lasso`
- Clips: 3
- Anims: 3
- Sample clips: pack:/lasso_neck.clip, pack:/lasso_torso.clip, pack:/lasso_feet.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### mech_grapple@lasso@_male@_ambient@_healthy@mounted@_streamed.ycd.xml
- Dict: `mech_grapple@lasso@_male@_ambient@_healthy@mounted@_streamed`
- Clips: 21
- Anims: 11
- Bone refs: SKEL_L_HAND, SKEL_NECK0, SKEL_R_HAND
- Sample clips: pack:/struggle_loop_success_att.clip, pack:/struggle_success_vic.clip, pack:/struggle_loop_mid_att.clip, pack:/struggle_success_att.clip, pack:/struggle_loop_success_vic.clip, pack:/struggle_loop_fail_att.clip, pack:/exit_standing_att.clip, pack:/exit_left_vic.clip
- Sample anims: biped_q5@biped@0_0, biped_q5@biped@0_1, biped_q5@biped@0_7, biped_q5@biped@0_2, biped_q5@biped@0_6, biped_q5@biped@0_3, biped_q5@biped@0_8, biped_q5@biped@0_9

### mech_grapple@lasso@_male@_ambient@_healthy@mounted@intimidation@on_ass@_base.ycd.xml
- Dict: `mech_grapple@lasso@_male@_ambient@_healthy@mounted@intimidation@on_ass@_base`
- Clips: 6
- Anims: 4
- Bone refs: CP_L_Forearm, SKEL_NECK0
- Sample clips: pack:/enter_left_att.clip, pack:/enter_front_att.clip, pack:/enter_right_vic.clip, pack:/enter_right_att.clip, pack:/enter_front_vic.clip, pack:/enter_left_vic.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_3, biped_q5@biped@0_0

### mech_grapple@lasso@_male@_ambient@_healthy@mounted@intimidation@on_knees@_base.ycd.xml
- Dict: `mech_grapple@lasso@_male@_ambient@_healthy@mounted@intimidation@on_knees@_base`
- Clips: 6
- Anims: 4
- Bone refs: CP_L_Forearm, SKEL_NECK0
- Sample clips: pack:/enter_front_att.clip, pack:/enter_right_vic.clip, pack:/enter_right_att.clip, pack:/enter_front_vic.clip, pack:/enter_left_vic.clip, pack:/enter_left_att.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_3, biped_q5@biped@0_0

### mech_inventory@equip@fallback@base@lasso.ycd.xml
- Dict: `mech_inventory@equip@fallback@base@lasso`
- Clips: 4
- Anims: 4
- Sample clips: pack:/unholster.clip, pack:/holster.clip, pack:/w_unholster.clip, pack:/w_holster.clip
- Sample anims: biped_q5@biped@0_1, prop_q5@tr3@0_0, biped_q5@biped@0_2, biped_q5@biped@0_0

### mech_inventory@equip@fallback@base@unarmed@satchel@lasso.ycd.xml
- Dict: `mech_inventory@equip@fallback@base@unarmed@satchel@lasso`
- Clips: 2
- Anims: 3
- Sample clips: pack:/unholster.clip, pack:/holster.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### mech_inventory@equip@fallback@base@unarmed@satchel@lasso_gesture.ycd.xml
- Dict: `mech_inventory@equip@fallback@base@unarmed@satchel@lasso_gesture`
- Clips: 2
- Anims: 3
- Sample clips: pack:/unholster.clip, pack:/holster.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### mech_inventory@equip@fallback@crouch@unarmed@satchel@lasso.ycd.xml
- Dict: `mech_inventory@equip@fallback@crouch@unarmed@satchel@lasso`
- Clips: 2
- Anims: 3
- Sample clips: pack:/unholster.clip, pack:/holster.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### mech_inventory@equip@fallback@first_person@unarmed@satchel@lasso_gesture.ycd.xml
- Dict: `mech_inventory@equip@fallback@first_person@unarmed@satchel@lasso_gesture`
- Clips: 2
- Anims: 3
- Sample clips: pack:/unholster.clip, pack:/holster.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### mech_inventory@equip@vehicle@shared@seated@base@unarmed@satchel@lasso_gesture.ycd.xml
- Dict: `mech_inventory@equip@vehicle@shared@seated@base@unarmed@satchel@lasso_gesture`
- Clips: 2
- Anims: 3
- Sample clips: pack:/unholster.clip, pack:/holster.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### mech_jump@arms@lasso.ycd.xml
- Dict: `mech_jump@arms@lasso`
- Clips: 1
- Anims: 3
- Sample clips: pack:/hand_grip.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### mech_melee@lasso@_male@_ambient@_healthy@_noncombat.ycd.xml
- Dict: `mech_melee@lasso@_male@_ambient@_healthy@_noncombat`
- Clips: 31
- Anims: 9
- Bone refs: SKEL_L_HAND, SKEL_R_HAND
- Sample clips: pack:/shove_running_from_back_dist_far_v1_vic.clip, pack:/attack_kick_push_rightside_dist_close_v1.clip, pack:/takedown_hogtie_from_right_v1_att.clip, pack:/attack_kick_stomp_leftside_dist_far_v1.clip, pack:/shove_running_from_front_dist_far_v1_att.clip, pack:/attack_kick_stomp_rightside_dist_near_v1.clip, pack:/takedown_hogtie_from_back_v1_vic.clip, pack:/takedown_hogtie_from_front_v1_att.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_4, biped_q5@biped@0_6, biped_q5@biped@0_7, biped_q5@biped@0_3, biped_q5@biped@0_5, biped_q5@biped@0_2, biped_q5@biped@0_8

### mega_mech_grapple@lasso@male@mounted.ycd.xml
- Dict: `mega_mech_grapple@lasso@male@mounted`
- Clips: 36
- Anims: 13
- Bone refs: SKEL_L_HAND, SKEL_NECK0, SKEL_R_HAND
- Sample clips: pack:/mech_grapple@lasso@_male@_ambient@_healthy@mounted@_base/facedown_enter_right_vic.clip, pack:/mech_grapple@lasso@_male@_ambient@_healthy@mounted@_base/running_tackle_from_back_running_trans_mount_att.clip, pack:/mech_grapple@lasso@_male@_ambient@_healthy@mounted@_base/facedown_enter_backleft_vic.clip, pack:/mech_grapple@lasso@_male@_ambient@_healthy@mounted@_base/running_tackle_from_right_running_trans_mount_vic.clip, pack:/mech_grapple@lasso@_male@_ambient@_healthy@mounted@_base/running_tackle_from_left_standing_trans_mount_vic.clip, pack:/mech_grapple@lasso@_male@_ambient@_healthy@mounted@_base/running_tackle_from_left_running_trans_mount_vic.clip, pack:/mech_grapple@lasso@_male@_ambient@_healthy@mounted@_base/facedown_enter_right_att.clip, pack:/mech_grapple@lasso@_male@_ambient@_healthy@mounted@_base/running_tackle_from_front_standing_trans_mount_vic.clip
- Sample anims: biped_q5@biped@0_11, biped_q5@biped@0_0, biped_q5@biped@0_1, biped_q5@biped@0_7, biped_q5@biped@0_2, biped_q5@biped@0_3, biped_q5@biped@0_8, biped_q5@biped@0_6

### mega_mech_strafe@generic@lasso.ycd.xml
- Dict: `mega_mech_strafe@generic@lasso`
- Clips: 109
- Anims: 16
- Sample clips: pack:/mech_strafe@generic@lasso@high_tension/stop_slow_ccw.clip, pack:/mech_strafe@generic@lasso@high_tension/move_slow_bwd.clip, pack:/mech_strafe@generic@lasso@low_tension/stop_slow_bwd.clip, pack:/mech_strafe@generic@lasso@mid_tension/move_fast_fwd.clip, pack:/mech_strafe@generic@lasso@low_tension/stop_fast_bwd.clip, pack:/mech_strafe@generic@lasso@high_tension/stop_fast_fwd.clip, pack:/mech_strafe@generic@lasso@mid_tension/move_fast_bwd.clip, pack:/mech_strafe@generic@lasso@mid_tension/move_slow_cw_close.clip
- Sample anims: biped_q5_finger_q0@biped@0_4, biped_q5_finger_q0@biped@0_12, biped_q5@biped@0_0, biped_q5_finger_q0@biped@0_8, biped_q5_finger_q0@biped@0_7, biped_q5_finger_q0@biped@0_1, biped_q5_finger_q0@biped@0_10, biped_q5@biped@0_1

### mega_mech_weapons_special@lasso.ycd.xml
- Dict: `mega_mech_weapons_special@lasso`
- Clips: 101
- Anims: 26
- Sample clips: pack:/mech_weapons_special@lasso@base@swing@sweep/aim_med_r90.clip, pack:/mech_weapons_special@lasso@base@ready@release/release_med_l90.clip, pack:/mech_weapons_special@lasso@base@pull@tighten_rope/release_fb_bwd_-135.clip, pack:/mech_weapons_special@lasso@base@pull@tighten_rope/release_fb_left_-45.clip, pack:/mech_weapons_special@lasso/idle_2_aim_fwd_med.clip, pack:/mech_weapons_special@lasso@base@release_wait@sweep/aim_med_0.clip, pack:/mech_weapons_special@lasso@base@ready@sweep/aim_med_0_intro.clip, pack:/mech_weapons_special@lasso@base@pull@tighten_rope/release_fb_right_45.clip
- Sample anims: biped_q5@biped@0_16, biped_q5@biped@0_11, biped_q5@biped@0_0, prop_q7@tr3@0_0, biped_q5@biped@0_22, biped_q5@biped@0_24, biped_q5@biped@0_13, biped_q5@biped@0_1

### script_mp@introflow@soloonfoot@lasso.ycd.xml
- Dict: `script_mp@introflow@soloonfoot@lasso`
- Clips: 24
- Anims: 8
- Sample clips: pack:/lasso_b_f_lasso_noose.clip, pack:/lasso_c_f_female.clip, pack:/lasso_b_m_lasso_bundle.clip, pack:/lasso_b_m_male.clip, pack:/lasso_a_m_male.clip, pack:/lasso_a_m_lasso_rope.clip, pack:/lasso_b_f_female.clip, pack:/lasso_a_m_lasso_noose.clip
- Sample anims: cinematic_q5@female@0_0, cinematic_q5@female@0_1, prop_q8@tr3@0_1, prop_q8@tr3@0_2, cinematic_q5@biped@0_0, cinematic_q5@biped@0_1, cinematic_q5@tr3@0_0, prop_q8@tr3@0_0

### script_mp@introflow@soloonhorse@lasso.ycd.xml
- Dict: `script_mp@introflow@soloonhorse@lasso`
- Clips: 16
- Anims: 10
- Sample clips: pack:/solo_lasso_b_lasso_bundle.clip, pack:/solo_lasso_a_lasso_rope.clip, pack:/solo_lasso_a_lasso_loop.clip, pack:/solo_lasso_c_mp_female_head.clip, pack:/solo_lasso_a_mp_female.clip, pack:/solo_lasso_c_mp_male.clip, pack:/solo_lasso_b_lasso_loop.clip, pack:/solo_lasso_c_lasso_bundle.clip
- Sample anims: cinematic_q5@female@0_0, cinematic_q5@female@0_1, cinematic_q5@biped@0_3, cinematic_q5@biped@0_4, cinematic_q5@biped@0_0, cinematic_q5@biped@0_1, cinematic_q5@biped@0_2, cinematic_q5@tr3@0_2

### script_mp@introflow@teamonfoot@lassos.ycd.xml
- Dict: `script_mp@introflow@teamonfoot@lassos`
- Clips: 125
- Anims: 24
- Sample clips: pack:/female_13_lassos_enter_f_player_face.clip, pack:/male_0_lassos_enter_bundle.clip, pack:/female_3_lassos_enter_bundle.clip, pack:/female_14_lassos_enter_f_player_face.clip, pack:/female_9_lassos_enter_noose.clip, pack:/female_6_lassos_enter_f_player.clip, pack:/female_5_lassos_enter_bundle.clip, pack:/female_12_lassos_enter_bundle.clip
- Sample anims: prop_q5@tr3@0_3, cinematic_q5@female@0_1, cinematic_q5@female@0_0, cinematic_q5@biped@0_5, cinematic_q5@biped@0_2, cinematic_q5@female@0_7, prop_q5@tr3@0_1, cinematic_q5@biped@0_1

### script_mp@introflow@teamonhorse@lassos.ycd.xml
- Dict: `script_mp@introflow@teamonhorse@lassos`
- Clips: 102
- Anims: 37
- Sample clips: pack:/intro_team_horse_lassos_female5.clip, pack:/intro_team_horse_lassos_female1.clip, pack:/intro_team_horse_lassos_lassoloop2.clip, pack:/intro_team_horse_lassos_male12.clip, pack:/intro_team_horse_lassos_female4.clip, pack:/intro_team_horse_lassos_male6.clip, pack:/intro_team_horse_lassos_female2.clip, pack:/intro_team_horse_lassos_lasso11.clip
- Sample anims: cinematic_q5@biped@0_13, cinematic_q5@female@0_1, cinematic_q5@female@0_4, cinematic_q5@tr3@0_3, cinematic_q5@biped@0_4, cinematic_q5@biped@0_10, cinematic_q5@female@0_5, cinematic_q5@biped@0_9

### veh_horseback@aim@front@special@lasso@base@loco.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@loco`
- Clips: 3
- Anims: 4
- Sample clips: pack:/idle.clip, pack:/cnt_idle.clip, pack:/wlk_idle.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_3, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@pull@loosen.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@pull@loosen`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_aim_0.clip, pack:/stn_aim_225l.clip, pack:/stn_aim_90r.clip, pack:/stn_aim_90l.clip, pack:/stn_aim_225r.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@pull@tighten_rope.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@pull@tighten_rope`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_release_0.clip, pack:/stn_release_225r.clip, pack:/stn_release_90l.clip, pack:/stn_release_225l.clip, pack:/stn_release_90r.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@pull@yank.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@pull@yank`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_aim_225l.clip, pack:/stn_aim_90r.clip, pack:/stn_aim_90l.clip, pack:/stn_aim_225r.clip, pack:/stn_aim_0.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@pull_off.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@pull_off`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_aim_0.clip, pack:/stn_aim_225l.clip, pack:/stn_aim_90r.clip, pack:/stn_aim_90l.clip, pack:/stn_aim_225r.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@ready.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@ready`
- Clips: 20
- Anims: 10
- Sample clips: pack:/stn_aim_0.clip, pack:/stn_release_225r.clip, pack:/stn_release_90r.clip, pack:/stn_release_0.clip, pack:/stn_aim_90l.clip, pack:/intro_225l.clip, pack:/intro_0.clip, pack:/intro_225r.clip
- Sample anims: biped_q5@biped@0_4, biped_q5@biped@0_1, biped_q5@biped@0_7, biped_q5@biped@0_5, biped_q5@biped@0_6, biped_q5@biped@0_2, biped_q5@biped@0_3, biped_q5@biped@0_9

### veh_horseback@aim@front@special@lasso@base@reelin.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@reelin`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_aim_0.clip, pack:/stn_aim_225l.clip, pack:/stn_aim_90r.clip, pack:/stn_aim_90l.clip, pack:/stn_aim_225r.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@reelin_drag.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@reelin_drag`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_aim_225r.clip, pack:/stn_aim_0.clip, pack:/stn_aim_225l.clip, pack:/stn_aim_90r.clip, pack:/stn_aim_90l.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@reelin_empty.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@reelin_empty`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_aim_225r.clip, pack:/stn_aim_0.clip, pack:/stn_aim_225l.clip, pack:/stn_aim_90r.clip, pack:/stn_aim_90l.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@reelin_empty_quick.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@reelin_empty_quick`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_aim_225r.clip, pack:/stn_aim_0.clip, pack:/stn_aim_225l.clip, pack:/stn_aim_90r.clip, pack:/stn_aim_90l.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@reelin_heavy.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@reelin_heavy`
- Clips: 5
- Anims: 4
- Sample clips: pack:/stn_aim_225r.clip, pack:/stn_aim_0.clip, pack:/stn_aim_225l.clip, pack:/stn_aim_90r.clip, pack:/stn_aim_90l.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_3, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@reelin_lead.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@reelin_lead`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_aim_225r.clip, pack:/stn_aim_0.clip, pack:/stn_aim_225l.clip, pack:/stn_aim_90r.clip, pack:/stn_aim_90l.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@reelin_pull.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@reelin_pull`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_aim_225r.clip, pack:/stn_aim_0.clip, pack:/stn_aim_225l.clip, pack:/stn_aim_90r.clip, pack:/stn_aim_90l.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@release_wait.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@release_wait`
- Clips: 5
- Anims: 4
- Sample clips: pack:/stn_aim_225r.clip, pack:/stn_aim_0.clip, pack:/stn_aim_225l.clip, pack:/stn_aim_90r.clip, pack:/stn_aim_90l.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_3, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@swing.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@swing`
- Clips: 10
- Anims: 3
- Sample clips: pack:/stn_release_90r.clip, pack:/stn_release_0.clip, pack:/stn_aim_225r.clip, pack:/stn_aim_0.clip, pack:/stn_release_225r.clip, pack:/stn_aim_225l.clip, pack:/stn_aim_90r.clip, pack:/stn_aim_90l.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@ready_rear_turn.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@ready_rear_turn`
- Clips: 6
- Anims: 3
- Sample clips: pack:/stn_transition_225r_to_90l.clip, pack:/stn_transition_225l_to_90r.clip, pack:/stn_transition_225r_to_0.clip, pack:/stn_transition_225r_to_225l.clip, pack:/stn_transition_225l_to_225r.clip, pack:/stn_transition_225l_to_0.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@ready_to_swing.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@ready_to_swing`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_transition_90l.clip, pack:/stn_transition_225r.clip, pack:/stn_transition_225l.clip, pack:/stn_transition_0.clip, pack:/stn_transition_90r.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@reelin_drag_rear_turn.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@reelin_drag_rear_turn`
- Clips: 6
- Anims: 3
- Sample clips: pack:/stn_transition_225l_to_90r.clip, pack:/stn_transition_225r_to_0.clip, pack:/stn_transition_225r_to_225l.clip, pack:/stn_transition_225l_to_225r.clip, pack:/stn_transition_225l_to_0.clip, pack:/stn_transition_225r_to_90l.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@reelin_drag_to_reelin_heavy.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@reelin_drag_to_reelin_heavy`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_transition_0.clip, pack:/stn_transition_90r.clip, pack:/stn_transition_90l.clip, pack:/stn_transition_225r.clip, pack:/stn_transition_225l.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@reelin_drag_to_reelin_lead.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@reelin_drag_to_reelin_lead`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_transition_90l.clip, pack:/stn_transition_225r.clip, pack:/stn_transition_225l.clip, pack:/stn_transition_0.clip, pack:/stn_transition_90r.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@reelin_heavy_rear_turn.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@reelin_heavy_rear_turn`
- Clips: 6
- Anims: 3
- Sample clips: pack:/stn_transition_225l_to_0.clip, pack:/stn_transition_225r_to_90l.clip, pack:/stn_transition_225l_to_90r.clip, pack:/stn_transition_225r_to_0.clip, pack:/stn_transition_225r_to_225l.clip, pack:/stn_transition_225l_to_225r.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@reelin_heavy_to_reelin.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@reelin_heavy_to_reelin`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_transition_90r.clip, pack:/stn_transition_90l.clip, pack:/stn_transition_225r.clip, pack:/stn_transition_225l.clip, pack:/stn_transition_0.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@reelin_heavy_to_reelin_drag.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@reelin_heavy_to_reelin_drag`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_transition_0.clip, pack:/stn_transition_90r.clip, pack:/stn_transition_90l.clip, pack:/stn_transition_225r.clip, pack:/stn_transition_225l.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@reelin_lead_rear_turn.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@reelin_lead_rear_turn`
- Clips: 6
- Anims: 3
- Sample clips: pack:/stn_transition_225l_to_0.clip, pack:/stn_transition_225r_to_90l.clip, pack:/stn_transition_225l_to_90r.clip, pack:/stn_transition_225r_to_0.clip, pack:/stn_transition_225r_to_225l.clip, pack:/stn_transition_225l_to_225r.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@reelin_lead_to_reelin.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@reelin_lead_to_reelin`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_transition_90l.clip, pack:/stn_transition_225r.clip, pack:/stn_transition_225l.clip, pack:/stn_transition_0.clip, pack:/stn_transition_90r.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@reelin_lead_to_reelin_drag.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@reelin_lead_to_reelin_drag`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_transition_90l.clip, pack:/stn_transition_225r.clip, pack:/stn_transition_225l.clip, pack:/stn_transition_0.clip, pack:/stn_transition_90r.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@reelin_rear_turn.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@reelin_rear_turn`
- Clips: 6
- Anims: 3
- Sample clips: pack:/stn_transition_225l_to_0.clip, pack:/stn_transition_225r_to_90l.clip, pack:/stn_transition_225l_to_90r.clip, pack:/stn_transition_225r_to_0.clip, pack:/stn_transition_225r_to_225l.clip, pack:/stn_transition_225l_to_225r.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@reelin_to_reelin_heavy.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@reelin_to_reelin_heavy`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_transition_0.clip, pack:/stn_transition_90r.clip, pack:/stn_transition_90l.clip, pack:/stn_transition_225r.clip, pack:/stn_transition_225l.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@reelin_to_reelin_lead.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@reelin_to_reelin_lead`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_transition_0.clip, pack:/stn_transition_90r.clip, pack:/stn_transition_90l.clip, pack:/stn_transition_225r.clip, pack:/stn_transition_225l.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@release_wait_rear_turn.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@release_wait_rear_turn`
- Clips: 6
- Anims: 3
- Sample clips: pack:/stn_transition_225r_to_90l.clip, pack:/stn_transition_225l_to_90r.clip, pack:/stn_transition_225r_to_0.clip, pack:/stn_transition_225r_to_225l.clip, pack:/stn_transition_225l_to_225r.clip, pack:/stn_transition_225l_to_0.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@swing_rear_turn.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@swing_rear_turn`
- Clips: 6
- Anims: 3
- Sample clips: pack:/stn_transition_225l_to_90r.clip, pack:/stn_transition_225r_to_0.clip, pack:/stn_transition_225r_to_225l.clip, pack:/stn_transition_225l_to_225r.clip, pack:/stn_transition_225l_to_0.clip, pack:/stn_transition_225r_to_90l.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0

### veh_horseback@aim@front@special@lasso@base@transitions@swing_to_ready.ycd.xml
- Dict: `veh_horseback@aim@front@special@lasso@base@transitions@swing_to_ready`
- Clips: 5
- Anims: 3
- Sample clips: pack:/stn_transition_90r.clip, pack:/stn_transition_90l.clip, pack:/stn_transition_225r.clip, pack:/stn_transition_225l.clip, pack:/stn_transition_0.clip
- Sample anims: biped_q5@biped@0_1, biped_q5@biped@0_2, biped_q5@biped@0_0
