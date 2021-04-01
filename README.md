Controlling the hotend / extruder cooling fan automatically.<br /> 
Requirements Marlin, PWM fan controll cct, Arduino mega / Ramps 1.4<br />
Connent the PWM driver circuit to D6 of Ramp 1.6 (Edit Configuration_adv.h making the following change <br> #define E0_AUTO_FAN_PIN -1 to #define E0_AUTO_FAN_PIN 6

<pre>
// @section extruder

// Extruder cooling fans
 // Extruder auto fans automatically turn on when their extruders'
 // temperatures go above EXTRUDER_AUTO_FAN_TEMPERATURE.
 // Your board's pins file specifies the recommended pins. Override those here
 // or set to -1 to disable completely.
 // Multiple extruders can be assigned to the same pin in which case
 // the fan will turn on when any selected extruder is above the threshold.

#define E0_AUTO_FAN_PIN 6
#define E1_AUTO_FAN_PIN -1
#define E2_AUTO_FAN_PIN -1
#define E3_AUTO_FAN_PIN -1
#define E4_AUTO_FAN_PIN -1
#define E5_AUTO_FAN_PIN -1
#define E6_AUTO_FAN_PIN -1
#define E7_AUTO_FAN_PIN -1
#define CHAMBER_AUTO_FAN_PIN -1

#define EXTRUDER_AUTO_FAN_TEMPERATURE 50
#define EXTRUDER_AUTO_FAN_SPEED 255   // 255 == full speed
#define CHAMBER_AUTO_FAN_TEMPERATURE 30
#define CHAMBER_AUTO_FAN_SPEED 255

</pre>

<br>
<br>
<br>
<br>
<br>
<br>
<br>
