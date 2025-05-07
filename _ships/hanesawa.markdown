---
layout: starship

ship_name: USS Hanesawa
image: "/assets/img/hanesawa_profile.jpg"
registry: NCC-47988
alignment: Starfleet
mission_profile: Multirole Explorer
service_record: 
  name: Dependable Workhorse
  detail: > 
    The ship is dependable, with a solid record of successful missions and accomplishments. While overshadowed by more famous ships, this vessel is nevertheless a mainstay of the fleet, with a competent, dedicated crew.
  trait: 
    name: Reliable
    detail: >
      Whenever the ship rolls to assist a task attempt, the group may spend 1 Momentum to ignore any complications rolled on the ship’s die.

class: Excelsior
scale: 5

shields: 19
resistance: 5
crew_support: 5

commission_year: 2371
launch_year: 2285
refits: 8

stats:
  systems:
    comms: 9
    engines: 10
    structure: 10
    computer: 9
    sensors: 11
    weapons: 9
  departments:
    command: 3
    engineering: 2
    medicine: 2
    conn: 2
    security: 4
    science: 2

attacks:
  - name: Phaser Banks
    type: Energy 
    range: Medium 
    damage: 8
    qualities: 
      - Versatile 2
  - name: Photon Torpedos
    type: Torpedo
    range: Long
    damage: 5
    qualities:
      - High Yield
  - name: Tractor Beam
    type: Tractor/Grappler
    range: Close
    damage: 4 

talents:
  - name: High-Resolution Sensors
    detail: >
      The vessel’s sensors can gain large amounts of accurate data, though they are extremely sensitive. While the vessel is not in combat, any successful task assisted by the ship’s Sensors gains 1 bonus Momentum. Bonus Momentum may not be saved.
  - name: Improved Warp Drive
    detail: >
      Whenever the ship takes the Warp major action, roll a d20; if you roll equal to or under the ship’s Engines, you do not spend Reserve Power for the ship.
  - name: Rugged Design
    detail: >
      Whenever a task roll is attempted to patch or repair a breach, a d20 may be re-rolled. Further, if the task is successful, the crew may spend Momentum to patch a second breach; this will cost 2 Momentum, +1 per additional step of Potency on that second breach.
  - name: Saucer Separation
    detail: >
      Vessels of this class have the capability to, detach their saucer section in an emergency. Once the saucer has detached, the two sections of the ship cannot be reconnected outside of a drydock. Ship’s systems are halved (round up) for the saucer and the secondary hull when separated, the saucer is unable to enter warp speeds or launch small craft, and each section is considered a separate vessel with Scale 1 less than the original vessel; the secondary hull is commanded from main engineering. The saucer can land on a planetary surface with emergency landing gear.
  - name: Secondary Reactors
    detail: > 
      The ship has additional impulse and fusion reactors which allow the ship to generate far greater quantities of energy. Once per scene, when you take the Reroute Power action, you may spend 2 Momentum (Immediate) to immediately regain the use of Reserve Power.
---

<img {% twoxify "/assets/img/hanesawa_msd.jpg" %} />
<img {% twoxify "/assets/img/hanesawa_bridge1.jpg" %} />
<img {% twoxify "/assets/img/hanesawa_bridge2.jpg" %} />