# GVHMR 根运动与泛化：自动汇报
完成物理评估 321/321；Demo 32。

五臂从同一个 GV-only 12000 步模型继续，使用相同训练来源和每步32个人/32个机器人锚点。DEV12用于开发；额外VAL43与训练隔离。

|阶段|模型|输入|完成/登记|完整/跌倒|关节rad|XY m|朝向°|世界MPJPE mm|
|---|---|---|---|---|---|---|---|---|
|1500|r38_A_continue_estimated|human|12/12|12/0|0.0959|0.2401|15.5225|280.8496|
|1500|r38_B_freeze_estimated|human|12/12|12/0|0.0948|0.2294|14.3802|271.1626|
|1500|r38_C_root_estimated|human|12/12|12/0|0.0964|0.2549|13.9322|295.2275|
|1500|r38_D_aug_estimated|human|12/12|12/0|0.0962|0.2436|17.9897|283.2227|
|1500|r38_E_combo_estimated|human|12/12|12/0|0.0962|0.2553|18.1701|291.2784|
|6000|r38_A_continue_VAL43|human|43/43|43/0|0.1522|0.0443|6.4162|67.4409|
|6000|r38_A_continue_estimated|human|12/12|12/0|0.0929|0.2431|18.3050|281.5517|
|6000|r38_A_continue_paired_robot|paired_robot|12/12|12/0|0.1188|0.3837|34.4681|446.5631|
|6000|r38_B_freeze_estimated|human|12/12|12/0|0.0921|0.2446|18.0882|289.5032|
|6000|r38_B_freeze_paired_robot|paired_robot|12/12|12/0|0.1204|0.3676|33.7776|434.4797|
|6000|r38_C_root_estimated|human|12/12|12/0|0.0923|0.2472|19.3318|285.5030|
|6000|r38_C_root_paired_robot|paired_robot|12/12|12/0|0.1189|0.3528|32.6954|429.6994|
|6000|r38_D_aug_estimated|human|12/12|12/0|0.0917|0.2383|17.4619|277.5032|
|6000|r38_D_aug_paired_robot|paired_robot|12/12|12/0|0.1201|0.3650|33.5917|434.3898|
|6000|r38_E_combo_estimated|human|12/12|12/0|0.0906|0.2285|15.9573|269.6832|
|6000|r38_E_combo_paired_robot|paired_robot|12/12|12/0|0.1188|0.3774|31.8661|447.2883|
|6000|r38_F_expand48_DEV12|human|12/12|12/0|0.0932|0.2138|15.2358|261.0159|
|6000|r38_F_expand48_VAL43|human|43/43|43/0|0.1238|0.0422|6.3375|60.9673|
|12000|r37_parent_VAL43|human|43/43|43/0|0.1507|0.0506|7.1462|77.0202|

## 直接观看
- [同预算续训：MoVi_F_S55_running_in_spot_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/同预算续训_阶段6000_MoVi_F_S55_running_in_spot_part2_v1.mp4)
- [同预算续训：MoVi_F_S55_sideways_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/同预算续训_阶段6000_MoVi_F_S55_sideways_part2_v1.mp4)
- [同预算续训：MoVi_F_S56_jogging_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/同预算续训_阶段6000_MoVi_F_S56_jogging_part2_v1.mp4)
- [同预算续训：MoVi_F_S57_jogging_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/同预算续训_阶段6000_MoVi_F_S57_jogging_part2_v1.mp4)
- [同预算续训：MoVi_F_S58_running_in_spot_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/同预算续训_阶段6000_MoVi_F_S58_running_in_spot_part2_v1.mp4)
- [同预算续训：MoVi_F_S58_walking_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/同预算续训_阶段6000_MoVi_F_S58_walking_part2_v1.mp4)
- [同预算续训：MoVi_F_S59_running_in_spot_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/同预算续训_阶段6000_MoVi_F_S59_running_in_spot_part2_v1.mp4)
- [固定共享命令接口：MoVi_F_S55_sideways_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/固定共享命令接口_阶段6000_MoVi_F_S55_sideways_part2_v1.mp4)
- [固定共享命令接口：MoVi_F_S56_jogging_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/固定共享命令接口_阶段6000_MoVi_F_S56_jogging_part2_v1.mp4)
- [固定共享命令接口：MoVi_F_S58_walking_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/固定共享命令接口_阶段6000_MoVi_F_S58_walking_part2_v1.mp4)
- [固定共享命令接口：MoVi_F_S59_jogging_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/固定共享命令接口_阶段6000_MoVi_F_S59_jogging_part2_v1.mp4)
- [固定共享命令接口：MoVi_F_S59_walking_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/固定共享命令接口_阶段6000_MoVi_F_S59_walking_part2_v1.mp4)
- [加强根运动监督：MoVi_F_S55_running_in_spot_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/加强根运动监督_阶段6000_MoVi_F_S55_running_in_spot_part2_v1.mp4)
- [加强根运动监督：MoVi_F_S56_jogging_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/加强根运动监督_阶段6000_MoVi_F_S56_jogging_part2_v1.mp4)
- [加强根运动监督：MoVi_F_S57_jogging_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/加强根运动监督_阶段6000_MoVi_F_S57_jogging_part2_v1.mp4)
- [加强根运动监督：MoVi_F_S58_walking_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/加强根运动监督_阶段6000_MoVi_F_S58_walking_part2_v1.mp4)
- [加强根运动监督：MoVi_F_S59_jogging_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/加强根运动监督_阶段6000_MoVi_F_S59_jogging_part2_v1.mp4)
- [输入噪声与时间遮罩：MoVi_F_S55_sideways_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/输入噪声与时间遮罩_阶段6000_MoVi_F_S55_sideways_part2_v1.mp4)
- [输入噪声与时间遮罩：MoVi_F_S56_jogging_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/输入噪声与时间遮罩_阶段6000_MoVi_F_S56_jogging_part2_v1.mp4)
- [输入噪声与时间遮罩：MoVi_F_S58_running_in_spot_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/输入噪声与时间遮罩_阶段6000_MoVi_F_S58_running_in_spot_part2_v1.mp4)
- [输入噪声与时间遮罩：MoVi_F_S59_jogging_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/输入噪声与时间遮罩_阶段6000_MoVi_F_S59_jogging_part2_v1.mp4)
- [输入噪声与时间遮罩：MoVi_F_S59_sideways_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/输入噪声与时间遮罩_阶段6000_MoVi_F_S59_sideways_part2_v1.mp4)
- [固定接口与根运动及泛化：MoVi_F_S55_running_in_spot_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/固定接口与根运动及泛化_阶段6000_MoVi_F_S55_running_in_spot_part2_v1.mp4)
- [固定接口与根运动及泛化：MoVi_F_S57_walking_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/固定接口与根运动及泛化_阶段6000_MoVi_F_S57_walking_part2_v1.mp4)
- [固定接口与根运动及泛化：MoVi_F_S58_running_in_spot_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/固定接口与根运动及泛化_阶段6000_MoVi_F_S58_running_in_spot_part2_v1.mp4)
- [固定接口与根运动及泛化：MoVi_F_S58_walking_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/固定接口与根运动及泛化_阶段6000_MoVi_F_S58_walking_part2_v1.mp4)
- [固定接口与根运动及泛化：MoVi_F_S59_sideways_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/固定接口与根运动及泛化_阶段6000_MoVi_F_S59_sideways_part2_v1.mp4)
- [r37_parent_VAL43：MoVi_F_S56_throw_catch_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/r37_parent_VAL43_阶段12000_MoVi_F_S56_throw_catch_part2_v1.mp4)
- [r37_parent_VAL43：MoVi_F_S57_hand_waving_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/r37_parent_VAL43_阶段12000_MoVi_F_S57_hand_waving_part2_v1.mp4)
- [扩展真人训练动作：MoVi_F_S57_jogging_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/扩展真人训练动作_阶段6000_MoVi_F_S57_jogging_part2_v1.mp4)
- [扩展真人训练动作：MoVi_F_S57_walking_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/扩展真人训练动作_阶段6000_MoVi_F_S57_walking_part2_v1.mp4)
- [扩展真人训练动作：MoVi_F_S59_sideways_part2_v1](/cephfs_ssd_xumengdi/video2action_migration_20260927/root/autodl-tmp/video2action-rl/科研汇报_20260917至20261103/15_GVHMR根运动与泛化_20261106/Demo/扩展真人训练动作_阶段6000_MoVi_F_S59_sideways_part2_v1.mp4)
