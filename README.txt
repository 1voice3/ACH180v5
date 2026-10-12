ACH180 Trainer - single file version (v5: all parameters, Carrier 2-speed retrofit lesson, PID lesson)
Upload index.html to the ROOT of a GitHub repo (delete old files first), then Settings > Pages > Deploy from a branch > main / root.
Open https://YOUR-USERNAME.github.io/YOUR-REPO/ in Safari, then Share > Add to Home Screen. Needs a connection to open.

Independent training simulator. Not ABB or Carrier. It controls no equipment and does not replace the manuals or the retrofit guide.

NEW IN THIS VERSION
- All 946 numbered parameters of firmware manual 3AXD50000955893 Rev B are editable (selections, numbers, hex bit fields, free values) on the
  Params tab and on the panel (Main menu > Parameters). Groups 01-09 and the other read-only signals show live values where the simulation has them.
  About 80 writable parameters change the simulation; the rest are stored, range checked and shown. Extraction from the PDF is not hand-verified.
- 96.04 Macro select, 96.06 Parameter restore and 96.07 Parameter save manually act and revert to Done (0) by themselves, as on the drive.
  Parameters the manual marks "cannot be changed while the drive is running" refuse changes until you press Off.
- Learn tab, three lessons:
  1. HVAC macro start-up (the original exercise, unchanged).
  2. Carrier 2-speed retrofit (ACH550 to ACH180): the guide's steps 1-10 in order, wiring table, motor data tag with BHP sticker (several tags),
     parameter table with order checks (96.04 first, 96.07 last), then a check-out: 40 Hz on DI2, 60 Hz on DI3.
  3. PID supply fan: the manual's "Supply fan, PID control" example (EXT2, AI1 setpoint, AI2 transducer, start interlocks 1 and 2, RO1 running).
     ACH180 96.04 has only Done and HVAC default, so the PID lesson is a wiring and parameter example, not a macro.
- Wiring tab: AI2, five field contacts, STO jumpers (5091 Safe torque off), line and motor power cables, DCOM and rail wiring.
- Panel tab: disconnect (power) switch, duct load slider with a simple fan-law process so the PID loop really settles.

Simplified models (training only): ramps, current, overload timing, PID scaling and tuning response, duct pressure, macro reload scope
(this trainer reloads defaults for every group except 95 and 96), and wiring rules.
Not modeled: vector control, fieldbus, timed functions, supervision functions, motor potentiometer, DI5, the other parameters' internal effects.
