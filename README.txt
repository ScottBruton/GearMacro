Gear Macro — paste into Spur gear 2021.swp (7 VBA modules):

  Involute1      Involute1.txt       entry, globals, DebugPrint, GenerateGear
  UserForm1      UserForm1_Code.txt  UI
  MasterSketch   MasterSketch.txt    layout sketch
  GearBody       GearBody.txt        revolve + fillet
  Tooth          Tooth.txt           gap sketch + cut
  Pattern        Pattern.txt         circular pattern
  GearLib        GearLib.txt         shared code + gear train (no DebugPrint here)

After paste: Debug → Compile VBAProject (must succeed with zero errors).
DebugPrint exists only in Involute1. Remove any duplicate Sub DebugPrint from other modules.

GenerateGear: MasterSketch -> axis -> GearBody -> Tooth -> Pattern -> validate -> equations

Supports: driving / driven / stacked gears, external & internal, parametric equations.
