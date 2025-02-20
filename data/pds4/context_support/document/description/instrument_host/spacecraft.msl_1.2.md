
 
 
  Instrument Host Overview
  ========================
    During the MSL mission, data are collected by instruments on the rover
    and those data are relayed directly to stations of the NASA Deep Space
    Network (DSN) on Earth or indirectly to the DSN using the orbital relay
    capability of Mars Reconnaissance Orbiter (MRO) or 2001 Mars Odyssey
    (ODY). The following sections provide an overview of the MSL
    spacecraft, DSN ground system, and MRO and ODY orbiters.
 
 
  Instrument Host Overview - Rover
  ================================
    The Mars Science Laboratory (MSL) mission landed a mobile science
    laboratory on Mars to assess the biological potential of the landing
    site, characterize the geology of the landing region, investigate
    planetary processes that influence habitability, and characterize
    the broad spectrum of radiation.  For more detailed information
    about the MSL spacecraft, see [GROTZINGER2009, GROTZINGERETAL2012].
 
 
    Spacecraft Configuration for Cruise and Approach
    ------------------------------------------------
      Following launch of the MSL flight system, the cruise stage
      separated from the launch vehicle and headed to Mars.  On its way,
      the spin-stabilized spacecraft performed 4 trajectory correction
      maneuvers (TCMs) and underwent a series of checkout and maintenance
      activities.  A health checkout of each of the science instruments
      plus the engineering cameras was carried out from March 12 to 22,
      2012, beginning 108 days after launch.  The one exception to this is
      RAD, which was checked out and began routine science observations on
      December 6, 10 days after launch.  Additional late cruise checkouts
      were performed on Mastcan, MARDI, MAHLI and the engineering cameras
      on April 20, 2012; Mastcam, MARDI and MAHLI plus the engineering
      cameras and REMS were checked again on June 14, 2012; the SAM
      instrument was checked on June 28, 2012.
 
 
    Spacecraft Configuration for Entry, Descent, and Landing
    --------------------------------------------------------
      After separation from the cruise stage, the 2559 kg entry vehicle,
      consisting of the backshell and heat shield enclosing the descent
      stage and rover, performed a series of guided maneuvers. Cruise
      balance masses separated to adjust the center of mass of the entry
      vehicle.  At 3522.2 km from the center of Mars, the vehicle entered
      the atmosphere.  This was followed by peak heating, peak
      deceleration, supersonic parachute deploy, and heat shield
      separation.  At the appropriate time, the descent stage engines
      started, the backshell and parachute separated, and the MARs Descent
      Imager (MARDI) started recording video.  As the descent stage
      approached the surface using powered descent, at an altitude of
      about 18.6 m, the rover was lowered on a descent rate limiter and
      bridle umbilical device to 7.5 m below the descent stage, and its
      wheels were deployed into the touchdown configuration. The descent
      stage continued descending until the rover touched down on the
      surface of Mars. The rover landed in Gale Crater at 15:03 Local Mean
      Solar Time on Mars (August 6, 2012, 05:18 UTC Spacecraft Event
      Time).  Upon successful touchdown, the descent rate limiter and
      bridle umbilical device were cut. The descent stage flew away and
      impacted the surface 650 meters away from the rover.
 
 
    Rover on the Surface of Mars
    ----------------------------
      After landing, the instrument host is the rover.  Overall
      characteristics of the rover include a total mass of ~900 kg, 2.8
      m width, 3 m length (4.7 m long with robotic arm extended), 1.1 m
      top deck height, 2.2 m total height, and 84 kg instrument payload.
      The rover is a vehicle for remote operation on the Martian surface
      with the following capabilities: (1) supports the science
      instrument payload investigations, (2) can traverse up to 100 to
      200 meters per sol, depending on the terrain, (3) provides high-
      speed computational capability and substantial data storage, and
      (4) provides X-band for Direct-to- Earth (DTE) and Direct-from-
      Earth (DFE) telecommunications, and the ability to communicate via
      UHF with Mars Reconnaissance Orbiter and Mars Odyssey (which will
      store and relay data to the Earth).
 
      The rover is a scaled version of the 6-wheel drive, 4-wheel
      steering system from the Mars Exploration Rover (MER).  Based on
      the center of mass, the vehicle is required to withstand a static
      tilt of at least 50 deg in any direction without overturning.  Fault
      protection will limit the rover from exceeding 30 deg tilts while
      driving.  The design of the rocker-bogie allows the wheels to move
      over objects approximately as large as the wheel diameter (0.5 m).
      Clearance under the rover's body on flat ground is 66 cm.  Each
      wheel has cleats and is independently actuated and geared,
      providing for climbing in soft sand and scrambling over rocks.
      Each front and rear wheel can be independently steered, allowing
      the vehicle to turn in place as well as execute arcing turns.  The
      rover has a top speed on flat hard ground of ~4 cm/s but under
      autonomous control with hazard avoidance, the vehicle achieves an
      average speed of ~1.5 cm/s.
 
      Rover power is provided by the Multi-Mission Radioisotope
      Thermoelectric Generator (MMRTG), which generates ~110 W of
      electrical power at the start of the landed mission.  Peak power
      demand from the rover activities easily exceeds this however, and
      the rover has two Li-Ion rechargeable ~42 amp-hour batteries to
      allow for all activities.  The batteries go through multiple
      charge/discharge cycles per Sol, with maximum allowed depth of
      discharge of ~53%.
 
      The surface telecommunications system uses three antennas, two for
      X-Band DTE/DFE (Direct to/from Earth), and a UHF antenna for relay
      to an orbiting asset.  The X-band antennas are the Rover Low Gain
      Antenna (RLGA) and the High Gain Antenna (HGA).  The HGA is used for
      either direct-to-Earth (DTE) or direct-from-Earth (DFE), while the
      RLGA is used primarily for DFE.  The basic telecom requirement for
      surface operations on the HGA is to transmit at least at 160 bits
      per second to a 34-meter Deep Space Network (DSN) antenna, or 800
      bits per second to a 70-meter DSN antenna.  In safe mode, commands
      from the Earth are received via the LGA, which does not require
      pointing.  Limited capability for communications exists via the LGA
      (15 bits per second uplink at max range). Typical daily uplink of
      commands is done via the HGA, taking approximately 15 minutes for a
      total volume of 225 kilobits.  The HGA sits on a 2 degree-of-freedom
      gimbal, with 5 degree system pointing accuracy (including rover
      attitude knowledge), and is 0.28 meters in diameter.
 
      The primary data return path for surface operations is via the UHF
      relay system, using the Mars orbiting assets, Mars Odyssey and Mars
      Reconnaissance Orbiter (MRO).  The project intends for primary
      communications to go through MRO, with two passes a day primarily
      used to return data from the surface.  Typically, it is expected
      that science decisions will be supported by returning a minimum of
      50 to 100 megabits of low-latency decision-supporting data for the
      tactical process, and up to 800 total megabits of data per sol.  The
      mission is designed to work with a minimum of 250 megabits per sol
      using two UHF passes.  Communications with Odyssey are subject to
      necessity and available energy.  The UHF subsystem has a pair of
      redundant Electra-Lite radios.  If for any reason DTE/DFE via X-Band
      is not possible, the UHF passes can be used to command the rover
      instead. A single quad-helix antenna called the RUHF is mounted to
      the rover deck and used for either of the radios.
 
      The computing, command, data handling, power regulation, and power
      distribution functions of the rover (for all phases of the mission
      including cruise and EDL) are supported by two identical computers
      (two for redundancy backup) called Rover Compute Elements (RCEs).
      Each computer has a 32-bit RAD750 processor which is capable of up
      to 400 MIPS.  Each RCE contains a central processor (a radiation
      hardened PowerPC 750 architecture system) that communicates with
      peripheral devices using other cards connected on a compact PCI
      backplane interface, and provides central memory storage for mission
      data and telemetry of 32 Gb via a Non-Volatile Memory / Camera
      (NVMCAM) card. In addition to the RCEs, power switching and analog
      input/output is provided by the redundant Rover Power and Analog
      Modules (RPAMs) connected to the RCEs. Battery charge management is
      provided via the two Battery Control Boards (BCBs) with one BCB for
      each battery.  The Rover Motor Control Assembly (RMCA) contains
      drivers for controlling all engineering actuators. Up to eight
      actuators can be driven simultaneously. The software in the main
      computer of the rover executes a control loop which monitors the
      status of the flight system during all phases, checks for the
      presence of commands to execute, maintains a buffer of telemetry for
      transmission, performs communication functions, and checks the
      overall health of the spacecraft.
 
      On the surface, activities such as imaging, driving, or instrument
      operations are performed under commands transmitted in a command
      sequence to the rover from the flight team.  The rover generates
      constant Engineering, Housekeeping and Analysis (EH&A) telemetry
      and episodic Event Reports (EVR) that are stored for eventual
      transmission.
 
      There are four main types of science instruments on the rover: (1)
      the contact instruments APXS (Alpha-Particle X-ray Spectrometer) and
      MAHLI (Mars Hand Lens Imager) on the end of the robotic arm; (2) the
      remote sensing instruments ChemCam (Chemical Camera) and Mastcam
      (Mast Cameras) mounted on the mast; (3) the environmental
      instruments DAN (Dynamic Albedo of Neutrons), MARDI (Mars Descent
      Imager), RAD (Radiation Assessment Detector), and REMS (Rover
      Environmental Monitoring Station); and (4) the analytical laboratory
      instruments CheMin (Chemistry and Mineralogy) and SAM (Sample
      Analysis at Mars), which are inside the body of the rover.
 
      In addition to the science cameras, the MSL rover carries 12
      engineering cameras (4 Navcams and 8 Hazcams), all of which share
      the same design as those on the Mars Exploration Rovers Spirit and
      Opportunity (see [Makietal2003]).  The primary set of engineering
      cameras is a Navcam pair near the top of the mast, a front Hazcam
      pair mounted on the front panel of the rover body and a rear
      Hazcam pair mounted on the back panel.  Three pairs of the cameras
      provide redundant backups (an extra Navcam pair and an extra Front
      and Rear Hazcam pair). The redundant backup cameras are connected
      to the backup rover computer and are not expected to be used
      unless there is a problem with the primary rover computer and/or
      primary cameras.
 
      The Remote Sensing Mast (RSM), provides a tall geologist's eye-
      level view from the cameras mounted at the top, ~2 meters above
      the Martian surface.  The RSM head includes the ChemCam, Mastcams,
      and Navcams, with the ChemCam sitting inside of the remote warm
      electronics box (R-WEB).  The R-WEB is a thermally controlled
      enclosure atop the mast.  The RSM has the ability for azimuth and
      elevation control, and can slew at 5 degrees per second.  The RSM
      allows for full 360 degree (plus or minus 181 degree) azimuth and
      plus or minus 91 degree elevation (zenith to nadir) range of
      motion.  Mounted along the shaft of the mast are two booms for the
      REMS investigation.
 
      The Sample Acquisition, Processing, and Handling (SA/SPaH)
      subsystem is responsible for the acquisition of rock and soil
      samples from the Martian surface and the processing of these
      samples into fine particles that are then distributed to the
      analytical science instruments, SAM and CheMin.  The SA/SPaH
      subsystem is also responsible for the placement of the two contact
      instruments, APXS and MAHLI, on rock and soil targets.  SA/SPaH
      consists of a Robotic Arm (RA) and turret-mounted devices on the
      end of the arm, which include a drill, brush, soil scoop, sample
      processing device, and the mechanical and electrical interfaces to
      the two contact science instruments, APXS and MAHLI.  SA/SPaH also
      includes drill bit boxes, the Organic Check Material (OCM), and an
      observation tray, which are all mounted on the front of the rover,
      and inlet cover mechanisms that are placed over the SAM and CheMin
      solid sample inlet tubes on the rover top deck.
 
      The Robot Arm (RA) is a 5 degree-of-freedom manipulator that is
      used to place and hold the turret-mounted devices and instruments
      on rock and soil targets, as well as manipulate the turret-mounted
      sample processing hardware.  The 5 degrees of freedom are provided
      by a set of rotary actuators known as the shoulder azimuth joint,
      the shoulder elevation joint, the elbow joint, the wrist joint,
      and the turret joint.  The joints are connected by structural
      elements with long links connecting the shoulder and elbow joints
      (known as the upper arm link) and connecting the elbow and wrist
      joints (known as the forearm link).  When fully extended straight
      ahead in the rover forward drive direction, the center of the
      turret of the robotic arm is 2.3 m from the front of the rover
      body.
 
      At the end of the RA is the turret structure on which 5 devices
      are mounted.  The outer diameter of the turret plus the installed
      devices is 60 cm.  Two of these devices are the science contact
      instruments APXS and MAHLI.  The remaining three devices are
      associated with sample acquisition and sample preparation
      function: the Powder Acquisition Drill System (PADS), Dust Removal
      Tool (DRT), and the Collection and Handling for Interior Martian
      Rock Analysis (CHIMRA).  The robotic arm can meet its positioning
      requirements for targets inside a volume called the robotic arm
      workspace.  The workspace volume is an upright cylinder 80 cm
      diameter, 100 cm high, positioned 105 cm in front of the front
      body of the rover, and extending to 20 cm below the surface when
      the rover is on a smooth flat terrain.
 
      The PADS is the device that is responsible for acquiring powdered
      rock samples from up to 5 cm inside the surface of a rock.  The
      drill both penetrates the rock and powders the sample to the
      appropriate size for analytical instrument use.  The powder
      travels up an auger in the drill and into a chamber with a
      transfer tube connection to the CHIMRA processing unit.  Movement
      of the powder through CHIMRA is driven by gravity (by changing the
      position and orientation of the robotic arm) and vibration.
 
      The diameter of the hole in a rock after drilling is 1.6 cm in
      diameter and up to 5 cm deep, depending on the surface topography of
      the rock.  Material from the upper ~1.5 cm of the drill hole is
      deposited on top of the rock surrounding the drill hole and does not
      make it into CHIMRA.
 
      The grain size distribution of the drilled powder and the
      temperatures to which the powder is heated during drilling will
      depend on the nature of the rock being drilled, the final drill
      design and performance, and operating parameters selected for use
      on Mars (rotation and percussion parameters, on-off cycles, etc).
      Pre-landing tests on prototype drills over a range of operational
      parameters and rock types have yielded samples with ~90% of the
      bulk material generated by the drill capable of passing through a
      150 um sieve and 100% passing through a 1 mm sieve.  Heating of
      the drilled sample in pre-landing tests was minimal.
 
      Soil samples are acquired with CHIMRA's clam-shell scoop
      mechanism, which can collect loose soil material from depths of up
      to 3.5 cm.  The volume of a scooped soil sample is expected to be
      between 1 and 30 cm3.
 
      The CHIMRA provides mechanisms for sieving particles to less than
      150 um, mixing the samples that pass through the 150 um sieve, and
      portioning the samples into the appropriate volume (~76 mm3
      per portion) for distribution to the SAM and CheMin instruments.
      The CHIMRA also provides the capability for sieving particles to
      less than 1 mm and portioning that material into an appropriate
      volume for distribution to the SAM instrument (45-130 mm3 per
      portion).
 
      The MSL rover surface navigation coordinate frame is right-handed,
      orthogonal, and defined by axes Xr, Yr, and Zr.
 
      -- +Zr axis is normal to the rover top deck plane and points down,
         from the top deck toward the wheels;
 
      -- +Xr axis is parallel to the rover top deck plane and points
         from the center of the top deck toward the RSM assembly;
 
      -- +Yr completes the right hand frame.
 
      The origin of the MSL rover navigation frame is centered directly
      between the centers of the two middle wheels.
 
 
  Instrument Host Overview - DSN
  ==============================
    The Deep Space Network (DSN) is a telecommunications facility managed
    by the Jet Propulsion Laboratory of the California Institute of
    Technology for the U.S. National Aeronautics and Space Administration
    (NASA).
 
    The primary function of the DSN is to provide two-way communications
    between the Earth and spacecraft exploring the solar system.  To carry
    out this function it is equipped with high-power transmitters, low-
    noise amplifiers and receivers, and appropriate monitoring and control
    systems.
 
    The DSN consists of three complexes situated at approximately equally
    spaced longitudinal intervals around the globe at Goldstone (near
    Barstow, California), Robledo (near Madrid, Spain), and Tidbinbilla
    (near Canberra, Australia).  Two of the complexes are located in the
    northern hemisphere while the third is in the southern hemisphere.
 
    Each complex includes several antennas, defined by their diameters,
    construction, or operational characteristics: 70-m diameter, standard
    34-m diameter, high-efficiency 34-m diameter (HEF), and 34-m beam
    waveguide (BWG).
 
    For more information see [ASMAR&RENZETTI1993] and [JPLD-19379].
 
 
  Instrument Host Overview - Mars Reconnaissance Orbiter
  ======================================================
    Mars Reconnaissance Orbiter (MRO) was designed and built by Lockheed
    Martin Space Systems.
 
    To meet its science objectives, MRO has seven scientific
    instruments: Mars Color Imager (MARCI), Mars Climate Sounder (MCS),
    High Resolution Imaging Science Experiment (HiRISE), Compact
    Reconnaissance Imaging Spectrometer for Mars (CRISM), Context Imager
    (CTX), and Shallow (Subsurface) Radar (SHARAD).
 
    An Electra UHF Communications and Navigation Package on MRO allows
    the spacecraft to act as a communications relay between the Earth
    and landers and rovers on the martian surface.
 
 
  Instrument Host Overview - 2001 Mars Odyssey
  ============================================
    The 2001 Mars Odyssey (ODY) spacecraft was designed and built by
    Lockheed Martin Astronautics (LMA).
 
    To meet its science objectives, Mars Odyssey has three primary
    instruments: Thermal Emission Imaging System (THEMIS); Gamma Ray
    Spectrometer (GRS), which includes the High Energy Neutron Detector
    (HEND); and Mars Radiation Environment Experiment (MARIE).
 
    In addition to transmitting data collected by ODY instruments and
    systems, the telecommunications system is used to relay data from
    Mars surface assets and measure their relative motion
    radiometrically in the 400 MHz frequency range.  For more
    information, see [JPLD-16303].

        