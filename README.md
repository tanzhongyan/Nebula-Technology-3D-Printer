# Nebula Technology COREXY 3D Printer (taobao)

## Description

This is an in-depth review regarding the most popular COREXY 3D Printer currently on [Taobao](https://item.taobao.com/item.htm?spm=a1z09.8149145.w4004-9653588878.3.400e6876iOqY7E&id=698708994651). It also contains useful marlin files and STLs required for this printer.
Coming in at 170USD before shipping, it has many upgrades and features compared to other COREXY printers out there for a fraction of the price. 

## Features

* Electronics
    * 360W 12V power supply
    * Motherboard
        * MKS GEN L V1.0
    * Stepper Drivers
        * TMC2209 (standalone) for X and Y Stepper Motors
        * A4988 for Z, Z2 and E0 Stepper Motors
        * Independent Dual Z control
    * ABL 
        * BL Touch Clone (3D Touch)
    * Titan Extruder Direct Drive Clone
    * MK8 Hotend
        * Generic 40W Heater Catridge
        * Generic 100k Thermistor
        * PID controlled
    * 300 x 300 Heated Bed
        * Bang-Bang controlled
    * MGN 12 Linear Rails for X and Y axis
    * Cooling Fans
        * 3010 Heatsink cooling Fan
        * 5015 Part Cooling Radial Fan

* Firmware
    * Ultimaker Cura 5.3.1
    * Marlin 2.1.2.1

## Comparison to Ender 5

Using Ender 5 as a comparison, there are a few noticeable upgrades. 
* Pros (Comared to Ender 5)
    * Linear Rails and Optical Shafts. Z rollers are notorious for causing binding and other issues
    * Direct Drive
    * Half the price. Ender 5 costing $550 USD

* Cons (Comared to Ender 5)
    * Lack support and community assistance. Most suitable for intermediate 3D Printing enthusiast
    * Takes approximately 40 hours of build time
    * You might be better off building other community sourced projects such as the Hypercube or Voron

## Issues

1. For non-mandarin speaking enthusiast, the project proves to be difficult as the tutorials, descriptions and after service are all in mandarin. 
2. The instructions lack some crucial information and requires some experience & research to solve.
3. There may be some missing parts. For us, we were lacking T8 lead screw nuts.
4. Insufficient tools provided.
5. The parts were all printed in PLA. STLs are also reserved for their private usage. We had to reverse engineer some of the provided parts.
6. Firmware provided did not work as intended. The language was in mandarin, encoder was reversed, direction of motors was reversed as well, X axis was now the Y axis and vice versa. We had to redo the marlin firmware to fix such issues.
7. Heated bed is not PID controlled, and takes 5 minutes to heat up.
8. The original power point was a 3 pin plug directly connecting between the power supply and the outlet socket. This was dangerous as there was no protective fuse and there were exposed wires.
9. Xloader firmware provided did not work.
10. Click to resume prompt after G29 ABL.

## Solutions

1. We used Google Translate to converse with the seller.
2. ChatGPT amd BingAI was effective in providing certain advice regarding marlin firmware configuration and issues faced.
3. As we had some CAD, Marlin and Cura experience, solving these issues took approximately 10 hours of troubleshooting.
4. Recommend to get a mosfet for the hotbed.
5. We bought a power switch socket with fuse and printed out a mount for it.
6. Kapton tape was essential in securing drooping wires.

## Conclusion

With increasingly advance 3D printyers, we must analyse and balance the cost to benefit that comes with cheaper DIY projects. Personally, we were looking to use this 3D printer with a [Fystec Enraged Rabbit Carrot Feeder](https://item.taobao.com/item.htm?spm=a21n57.1.0.0.70dd523cJbnjHU&id=681765751259&ns=1&abbucket=2#detail) to do multicoloured prints and prototyping. We spent an approximate of $370USD for the 3D Printer and Fystec ERCF. We spent 50 hours assembling just the 3D Printer alone. If you took into account cost to benefit, purchasing a [BambuLab P1S Combo](https://detail.tmall.com/item.htm?spm=a21n57.1.0.0.14d7523cgGgQYl&id=695623155242&ns=1&abbucket=2) off taobao would make more sense. The P1S would also retain its value for years to come. However, we were able to learn many useful skills such as methodical thought processes, problem solving and critical thinking. More technical skills such as how a 3D printer functions and operate, and software related competencies.

### TL;DR

* Pros
    * Learn technical skills and competencies regarding 3D printers
    * Low cost and affordable
    * Potentially better than other prebuild options
* Cons
    * Time extensive
    * Cost to benefit not worth it

## Authors

[@TanZhongYan](https://www.linkedin.com/in/zhong-yan-tan/)
[@HoKheeXuan](https://www.linkedin.com/in/ho-khee-xuan-a8a35b1b0/)

## License

This project is licensed under the [Creative Commons Attribution-NonCommercial-NoDerivatives (CC BY-NC-ND) License](LICENSE.md).

## Acknowledgments

* [Nebula Technology 3D Printing](https://shop115693462.taobao.com/shop/view_shop.htm?shop_id=115693462&spm=a21m98.27004841)
* [Marlin Firmware](https://marlinfw.org/)
* [Xloader](https://github.com/binaryupdates/xLoader)
