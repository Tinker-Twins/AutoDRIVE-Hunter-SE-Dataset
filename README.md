# AutoDRIVE Hunter SE Dataset

### Dynamics and Perception Dataset of "Hunter SE" Robot

<table>
<thead>
  <tr>
    <th align="center"><img src="straight_30_hz/straight.gif"></th>
    <th align="center"><img src="skidpad_30_hz/skidpad.gif"></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td align="center">Straight Track</td>
    <td align="center">Skidpad Track</td>
  </tr>
  <tr>
    <td align="center"><img src="fishhook_30_hz/fishhook.gif"></td>
    <td align="center"><img src="slalom_30_hz/slalom.gif"></td>
  </tr>
  <tr>
    <td align="center">Fishhook Track</td>
    <td align="center">Slalom Track</td>
  </tr>
</tbody>
</table>

This repository uses [AutoDRIVE Ecosystem](https://autodrive-ecosystem.github.io/) to capture data from a 1:5 scale Ackerman-steered vehicle called Hunter SE. The source repository for AutoDRIVE Ecosystem can be found [here](https://github.com/Tinker-Twins/AutoDRIVE).

## Dataset Structure:

The vehicle dataset comprises the following:

| **DATA** | timestamp | throttle |	steering | leftTicks | rightTicks |	posX | posY |	posZ | roll |	pitch |	yaw |	speed |	angX |	angY |	angZ | accX |	accY | accZ |
| -------- | --------- | -------- |	-------- | --------- | ---------- |	---- | ---- |	---- | ---- |	----- |	--- |	----- |	---- |	---- |	---- | ---- |	---- | ---- |
| **UNIT** | yyyy_MM_dd_HH_mm_ss_fff | norm% | rad | count | count |	m | m |	m | rad |	rad |	rad |	m/s |	rad/s |	rad/s |	rad/s | m/s^2 |	m/s^2 | m/s^2 |

## Vehicle Parameters:
- Wheelbase (m): 0.55
- Track width (m): 0.52
- Center of mass* (m): [x: 0.330, y: 0.000, z: 0.087]

  *Center of mass is measured w.r.t. the center of rear axle.
- Suspension stiffness (N/m): 22700
- Suspension damping (Ns/m): 7000
- Throttle Limit (norm%): 1.0000
- Steering Limit (rad): 0.5236
- Linear Velocity Limit (m/s): 3.5611
- Angular Velocity Limit (rad/s): 2.0708
- [Throttle vs. Velocity Mapping](https://github.com/Tinker-Twins/AutoDRIVE-Hunter-SE-Dataset/blob/main/vehicle_parameters/HunterSE_Throttle_Velocity_Mapping.xlsx):

  ![](https://github.com/Tinker-Twins/AutoDRIVE-Hunter-SE-Dataset/blob/main/vehicle_parameters/HunterSE_Throttle_Velocity_Mapping.png)
