## Tx Frame Id Assignments
- EPS: Static Slot 6 
- Drive Assist Front Camera: Dynamic Slot 65

## Signals
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
Range: [-540, 540] ???
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
Range: [-540, 540] ???
```

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

### LKAS Assist Torque Request
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
Torque Sensor Raw: 0x53
Torque Sensor: -1.66
Angle 1 Raw: 0x34a 
Angle 1: 128.826 
Angle 2 Raw: 0x35e 
Angle 2: 131.886

EPS Frame 2:
Offset: 00 01 02 03 04 05 06 07 08 09 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33
Data:   00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:24:03:00:00:41:0C:A5:33:3A:33:8A:0C:03:0E:00:00:00:70 
Torque Sensor Raw: 0xe
Torque Sensor: 0.28
Angle 1 raw: 0xc41 
Angle 1: -479.961 
Angle 2 raw: 0xc8a 
Angle 2: -491.13

Camera Frame 1:
Offset: 00 01 02 03 04 05 06 07 08 09 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33
Data:   60:00:40:4F:05:62:3B:4B:01:33:00:00:00:00:00:00:A1:0A:00:00:00:00:00:00:00:00:00:00:00:00:00:00:00:E0 
Assist Torque Request Raw: 0x133
Assist Torque Request: 0.07

Camera Frame 2:
Offset: 00 01 02 03 04 05 06 07 08 09 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33
Data:   60:00:40:4F:05:62:3B:4B:01:34:00:00:00:00:00:00:51:1F:FA:00:00:80:46:30:14:BF:0A:00:05:FE:07:00:00:F0 
Assist Torque Request Raw: 0x134
Assist Torque Request:0.08
```
