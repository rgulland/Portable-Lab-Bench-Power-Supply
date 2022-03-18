# Portable Lab Bench Power Supply
A mini lab bench power supply that values compactness and safety.  Details at https://rgulland.com/blog  
Assembled unit outputs up to 30V 5A ( digitally adjustable with OVP & OCP) to Banana jacks or XT60 in a <1L form factor.  BOM cost is around ~$100.

WARNING: This a hardware project that uses 120V AC mains power. It has not yet caught on fire, but there are absolutely no guarantees.

# Documentation
Design documentation:   https://rgulland.com/blog/2021/11/5/portable-power-supply-design
Assembly documentation: https://rgulland.com/blog/2021/11/10/portable-power-supply-assembly
Testing results:        https://rgulland.com/blog/2022/01/31portable-power-supply-testing

This is a heavily modified version of Kralyn3D's original 'DIY Mini Lab Bench Power Supply is available at https://www.youtube.com/watch?v=PhLFmokgr9o 
I personally don't recommend building the original version without reimplementing some of the AC safety features from this project (fuse, AC plug, digital power limit)

# Build Notes
Please don't build this unless you're confident working with mains power and have sufficient materials to do it safely.  
Please read all blogs before building.  
On initial power on, set a default power limit of 125-150W & 30.1V on the DSP5005 when using the AC input.  Above these limits, the AC-DC converter components will have a shorter life due to high temperatures. 

# LICENSE
This project is under the GPL v3 license.  There's little to no IP here, as most components are COTS, so this is more an endorsement of keeping more things open source. Open source hardware projects are rare, so if yours is, thanks :)  
https://www.gnu.org/licenses/gpl-3.0.en.html

# Todo
- .txt BOM & sourcing guide
- "AC Input" & "DC Input" emboss on frame near switch
- Support for cheaper / Aliexpress voltage converters instead of Pololu
- Source cheaper fan alternative to Noctua
- Add configuration for protruding 'banana sockets' that accept bare wires like standard lab-bench supplies
- v2 w/ custom AC-DC PCB with proper connectors, integrated fan speed control, etc
