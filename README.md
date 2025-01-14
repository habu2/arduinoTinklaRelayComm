# TeensyTinklaRelayComm
Allows one to have a Teensy 4.x device receive info from Tinkla Relay to control other devices

* Teensy needs to be powered separately and not from Tinkla Relay
* When controlling high output keep in mind the Teensy can only handle a max of 400mA when powered from USB
* If you intend to drive LED lights or other devices, please ensure you compute the total max comsumption from all your attached devices
* Overloading the Tinkla Relay can result in the failure of the device
* One should not request data from the Tinkla Relay more often than 4 times a seconf or the other functionality of the Relay might be affected

The following flags are read from Tinkla Relay
 - bool rel_option1_on
 - bool rel_option2_on
 - bool rel_option3_on
 - bool rel_option4_on
 - bool rel_car_on
 - bool rel_gear_in_reverse
 - bool rel_gear_in_forward
 - bool rel_left_turn_signal
 - bool rel_right_turn_signal
 - bool rel_brake_pressed
 - bool rel_highbeams_on
 - bool rel_light_on
 - bool rel_below_20mph
 - bool rel_left_steering_above_45deg 
 - bool rel_right_steering_above_45deg 
 - bool rel_AP_on 
 - bool rel_car_charging
 - bool rel_left_side_bsm
 - bool rel_right_side_bsm
 - bool rel_tacc_only_active
 - unsigned int rel_brightness
