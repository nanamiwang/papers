## Tx Frame Id Assignments
- EPS: Static Slot 6 
- Drive Assist Front Camera: Dynamic Slot 65

## Signals
### Steering Torque Sensor
```
Frame Id: 6
Start Bit: 29
Bit Length: 9
Endianess: Little Endian
Sign: Signed
Sign Mask: 0x80
Offset: 0
Scale: 0.02
Range: [-3.0, 3.0]
```

### Steering Assist Enabled Flag
```
Frame Id: 6
Start Bit: 28
Bit Length: 8
Endianess: Little Endian
Sign: Unsigned
Offset: 0
Scale: 1
Values: 
0x05 if LKA steering assist is enabled
0x03 if LKA steering assist is disabled
```

### Steering Angle Sensor 1
```
Frame Id: 6
Start Bit: 20
Bit Length: 12
Endianess: Little Endian
Sign: Signed
Sign Mask: 0x10
Offset: 0
Scale: 0.153
Range: [-540, 540]
```

### Steering Angle Sensor 2
```
Frame Id: 6
Start Bit: 26
Bit Length: 12
Endianess: Little Endian
Sign: Signed
Sign Mask: 0x80
Offset: 0
Scale: 0.153
Range: [-540, 540]
```

### LKA Assist Torque Request
```
Frame Id: 65
Start Bit: 8
Bit Length: 9
Endianess: Big Endian
Sign: Signed
Sign Mask: 0x10
Offset: 300 ???
Scale: 0.01 ???
Range: [-3.0, 3.0]
```

### Captured Frames Samples:
```
EPS Frame 1:
Offset: 00 01 02 03 04 05 06 07 08 09 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33
Data:   00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:17:08:00:00:4A:13:A4:33:D8:38:5E:83:03:53:80:00:00:70
Steering Assist Enabled: False
Steering Torque Sensor Raw: 0x53
Steering Torque Sensor: -1.66
Steering Angle 1 Raw: 0x34a 
Steering Angle 1: 128.826 
Steering Angle 2 Raw: 0x35e 
Steering Angle 2: 131.886

EPS Frame 2:
Offset: 00 01 02 03 04 05 06 07 08 09 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33
Data:   00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:24:03:00:00:41:0C:A5:33:3A:33:8A:0C:03:0E:00:00:00:70 
Steering Assist Enabled: False
Steering Torque Sensor Raw: 0xe
Steering Torque Sensor: 0.28
Steering Angle 1 raw: 0xc41 
Steering Angle 1: -479.961 
Steering Angle 2 raw: 0xc8a 
Steering Angle 2: -491.13

EPS Frame 3:
Offset: 00 01 02 03 04 05 06 07 08 09 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33
Data:   00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:6D:09:00:00:25:00:9A:33:56:39:25:00:05:15:00:00:00:70 
Steering Assist Enabled: True
Steering Torque Sensor Raw: 0x15 
Steering Torque Sensor: 0.42 
Steering Angle 1: raw 0x25 
Steering Angle 1: -5.661 
Steering Angle 2: raw 0x25 
Steering Angle 2: -5.661

Camera Frame 1:
Offset: 00 01 02 03 04 05 06 07 08 09 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33
Data:   60:00:40:4F:05:62:3B:4B:01:33:00:00:00:00:00:00:A1:0A:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:E0 
Assist Torque Request Raw: 0x133
Assist Torque Request: 0.07
```
