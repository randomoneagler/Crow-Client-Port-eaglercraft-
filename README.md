Crow b1.2.9 ported to EaglercraftX 1.8
The game file
EB_Client_1.8.html (27 MB) the REAL port, compiled from Java through
TeaVM. Double-click it (or host it anywhere) and it runs in your browser:
full Crow module set (KillAura family, Reach, Velocity, Speed/Fly, Scaffold,
Blink, InvManager, ChestStealer, HUD/Keystrokes/Nametags/ESP/TargetHUD,
Scoreboard, CustomHotbar, Crosshair, AutoGG, NameHider, Freecam, Terminal,
configs, 4 ClickGUI styles) 

Crow_1.8_Overlay_Legacy.html is the older JS-overlay experiment
(cosmetic only) was kept for reference, the new file supersedes it.

Source / for rebuilding
EB-Client-Eagler-Port.zip — the complete adapted source (~300 Java files),
the hook installer (tools/apply_port.py), and build docs (README.md
inside). Build step for dummies: clone the EaglercraftX 1.8 repo → BuildTools.jar workspace → run apply_port → CompileJS.sh → CompileEPK.sh →
MakeOfflineDownload.sh.

Crow-Eagler.zip is the earlier raw source dump (superseded by the port
package above).

Current Status 
Boots to the EaglercraftX profile screen, loads all 3974 resources
(incl. the Crow sounds/textures), initializes the full Crow client core
(98 modules + themes + commands + configs).
Known rough edge: the animated crow main menu is GPU-heavy; on very weak
software renderers it can stutter, and a GL_INVALID_ENUM console warning
may repeat (cosmetic). On normal hardware-accelerated browsers this is a
non-issue.

Notes

-very bad right now
