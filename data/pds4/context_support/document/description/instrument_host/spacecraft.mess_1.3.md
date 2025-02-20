
 
 
   Instrument Host Overview
   ========================
     The MErcury Surface, Space ENvironment, GEochemistry,
     and Ranging (MESSENGER) spacecraft was launched from
     the Cape Canaveral Air Station on 2004-08-03, on an
     approximately 8 year mission to become the first
     probe to orbit the planet Mercury. The initial mission
     included one year orbit of Mercury which was subsequently
     extended to a total of four years.
 
     Most of the science data collected by the MESSENGER
     mission will originate from instruments on the
     spacecraft and be relayed via the telemetry system to
     stations of the NASA Deep Space Network (DSN).  Radio
     Science (RS) experiments (Doppler velocity and ranging
     as well as radio occultations) require that DSN
     hardware also participate in the data acquisition.
     The following sections provide an overview first of
     the spacecraft, then of the DSN ground system, and
     the spacecraft clock reset and use of MET partitions.
 
     For more information on the spacecraft see
     [LEARYETAL2007]. For more information on the DSN see
     [ASMAR&RENZETTI1993].
 
 
   Instrument Host Overview - Spacecraft
   =====================================
     The MESSENGER spacecraft was built by the Johns
     Hopkins Applied Physics Laboratory (JHUAPL) to
     withstand the harsh environments encountered in
     achieving and operating in a Mercury orbit.  It can be
     divided into eight subsystems: structures and
     mechanisms; propulsion; thermal; power; avionics;
     software; guidance and control; radio frequency (RF)
     telecommunications, and payload.
 
     Structures and Mechanisms
     -------------------------
       The spacecraft's structures and mechanisms consist of
       the composite core structure, the aluminum launch
       vehicle adapter, and its deployables.
 
       The core of the spacecraft is the integrated
       structure/propulsion system. The structural load paths
       are optimized by using lightweight titanium fuel tanks
       designed specifically for the structural configuration
       chosen. The tank struts transfer lateral loads to the
       corners of the structure, allowing the use of
       composite panels that are thin relative to their size.
       The composite structure is designed to channel all
       loads into a center column, which necessitates a
       square-to-round launch vehicle adapter. This was a
       machined aluminum forging, carefully tailored to
       distribute evenly the structural loads from the
       corners of the center column to the round vehicle
       interface.
 
       The solar panel design and development effort proved
       to be challenging from a material engineering
       prospective. Extensive, ply-by-ply structural analysis
       was required for the solar array substrate due to the
       large cantilever in the stowed configuration and the
       use of high-conductivity, but relatively low-strength,
       graphite-cyanate ester (GrCE) materials in the
       sandwich face sheets.
 
       The sunshade support structure is welded titanium
       tubing construction. The tubing supports five
       antennas, the solar monitoring sensor for the X-Ray
       Spectrometer (XRS), four digital Sun sensors, and the
       sunshade. The final shape of the sunshade projected
       area was tailored to bring the center of solar
       pressure as close to the measured center of mass of
       the spacecraft as possible. By utilizing solar
       pressure, tilting the spacecraft relative to the Sun
       can unload the momentum wheels without expending fuel.
 
       Three mechanical assemblies required deployment: the
       two solar panels and the 3.6-m Magnetometer boom. The
       solar array panels were released first and allowed to
       settle; the arms were then released. The Magnetometer
       (MAG) boom deployment used the same sequence. After
       confirmation of full deployment, all six hinge-lines
       are pinned in place to prevent hinge rotation during
       high-thrust maneuvers.
 
     Propulsion
     ----------
       The spacecraft's propulsion subsystem consists of its
       state-of-the-art titanium fuel tanks, the thruster
       modules, and the associated plumbing.
 
       The subsystem is a pressurized bipropellant, dual-mode
       system using hydrazine (N2H4) and nitrogen tetroxide
       (N2O4) in the bipropellant mode and N2H4 in the
       monopropellant mode. Three main propellant tanks, a
       refillable auxiliary fuel tank, and a helium
       pressurant tank provide propellant and pressurant
       storage. The helium tank is a titanium-lined composite
       over-wrapped leak-before-burst pressure vessel (COPV)
       based on the flight-proven A2100 helium tank. A new
       lightweight main propellant tank was developed and
       qualified specifically for MESSENGER. The tank
       configuration is an all-titanium, hazardous-leak-
       before-burst design. A small 6Al-4V titanium auxiliary
       tank is a hazardous-leak-before-burst design. It has
       an internal diaphragm to allow positive expulsion of
       propellant for use in small burns.
 
       The propulsion subsystem includes a total of 17
       thrusters of three types. The large velocity adjustment
       (LVA) thruster is a flight-proven Leros-1b.  Four 22-N,
       monopropellant LVA-TVC thrusters provide thrust vector
       steering forces during main thrust burns and primary
       propulsion for most of the smaller velocity adjustment
       (delta-V) maneuvers.  Twelve monopropellant thrusters
       provide 4.4 N of thrust for fine attitude control
       burns, small delta-V burns, and momentum management.
 
       The propulsion thermal system employs heaters to
       maintain acceptable system temperatures. Heaters are
       used during the cruise phase to maintain propellant
       temperatures and in the operational phases to pre-heat
       thrusters in preparation for operation.
 
     Thermal
     -------
       The thermal subsystem consists of the spacecraft's
       ceramic-cloth sunshade, its heaters, and its
       radiators.
 
       The primary element of the thermal design is the
       ceramic-cloth sunshade, which protects the vehicle
       from the intense solar environment encountered when
       inside of Venus orbit. Creating a benign thermal
       environment behind the sunshade allowed for the use of
       essentially standard electronics, components, and
       thermal blanketing materials. Non-standard thermal
       designs were required for the solar arrays, sunshade,
       digital Sun sensors, three of the seven instruments,
       and the phased-array antennas. These components have
       been designed to operate at Mercury perihelion
       (Mercury closest to the Sun) and also during orbits
       that cross over one of Mercury's hot poles.
 
     Power
     -----
       The power subsystem consists of the spacecraft's solar
       arrays, battery, and the controlling electronics.
 
       The power subsystem utilizes a peak power tracker
       architecture that isolates the battery and the power
       bus from the variations of the solar array voltage and
       current characteristics and optimizes the solar array
       power output over the highly varied operating
       conditions of the mission. The power system is
       designed to support about 390 W of load power near
       Earth and 640 W during Mercury orbit.
 
       Because of the mission's large solar distance
       variations, the requirements placed on the solar array
       design are rather severe. The maximum solar array
       voltage during normal operations is expected to vary
       between 45 and 95 V, but this range does not include
       the higher transient voltages expected on the cold
       solar arrays at exits from eclipses. Triple junction
       solar cells are used. The solar cell strings are
       placed between Optical Solar Reflector (OSR) mirrors
       with a cell-to-OSR ratio of 1:2 to reduce the panel
       absorbance. Thermal control is performed by tilting
       the panels away from normal incidence with increased
       solar intensity. In case of an attitude control
       anomaly near Mercury, the solar array temperature may
       reach 270 degrees C. All material and processes used
       in the solar panels are designed to survive the worst-
       case predicted temperatures.
 
     Avionics
     --------
       The avionics subsystem consists of the spacecraft's
       processors, its solid-state data recorder, and the
       data handling electronics.  These components are
       packaged as an Integrated Electronics Module, or IEM.
 
       The IEM implements command and data handling (C&DH),
       guidance and control, and fault protection functions.
       Its design utilizes five daughter cards: the Main
       Processor (MP), the Fault Protection Processor (FPP),
       the 8-Gbit Solid-State Recorder (SSR), the Interface
       Card and the Converter Card.  These cards are tied
       together by a backplane, and a chassis utilizing the
       6U compact peripheral component interconnect (cPCI)
       standard.  Three of the cards (MP, FPP and SSR)
       implement fairly generic functions while the Interface
       and Converter Card are much more mission-specific.
 
       A primary driver of the IEM architecture was to
       simplify spacecraft fault protection. The FPP
       independently collects spacecraft health information
       which are continuously evaluated by a rule-based
       autonomy system. The FPP corrects faults by sending
       commands to the MP and other components. The IEM
       Interface board includes hardware limits to prevent a
       failed FPP from continuously sending commands that
       would disrupt the spacecraft operation.
 
     Software
     --------
       The software subsystem consists of the spacecraft's
       processor-supported code that performs command and
       data handling (C&DH), and spacecraft guidance and
       control (G&C). It consists of two applications, the MP
       and the FPP, implemented as C code under the VxWorks
       5.3.1 real-time operating system.
 
       The MP software implements all C&DH and G&C
       functionality in a single flight code application
       running on the MP card.
 
       The C&DH functionality includes uplink and downlink
       management, command processing and dispatch, support
       for stored and time-tagged commands, management of the
       SSR and file system, science data collection, image
       compression, telemetry generation, memory load and
       dump functions, and support for transmission of files
       from the SSR on the downlink using CCSDS File Delivery
       Protocol (CFDP).  It also collects analog temperatures
       and implements a peak power tracking algorithm to
       optimize charging of the spacecraft battery via a
       power subsystem interface.
 
       The G&C functionality maintains spacecraft attitude,
       manages spacecraft momentum, executes deep-space
       propulsive maneuvers, controls the solar arrays for
       optimized pointing to the Sun, manages spacecraft
       thermal environment by ensuring the sunshade always
       faces the Sun and enables a host of pointing options
       and instrument pointing control in support of science
       operations.
 
       The MP also contains a boot mode which supports
       rudimentary command processing and telemetry
       generation for reporting health status and to support
       uploads of code and parameters to EEPROM.
 
       The FPP application runs on the FPP card and
       implements an autonomy rule engine, which accepts
       uploadable health and safety rules that can operate on
       data collected from the various spacecraft subsystems
       via several interfaces, including an interface to the
       power subsystem. The action of each rule can dispatch
       commands to the MP or to the power subsystem to
       correct faults.
 
       Fault correction can include actions such as switching
       to redundant components, demotion to lower spacecraft
       modes (Safe Hold or Earth Acquisition), or shedding
       power loads. The FPP can swap the bus controller
       functionality between MPs, power on and switch to the
       redundant MP, select which of two stored applications
       the MP loads and can reset the MP.
 
       The spacecraft has two safing modes. During safing,
       all time-tagged command execution is halted and the
       spacecraft is taken to a pre-defined simple state.
       Safe Hold is the first level of safing and assumes
       knowledge of ephemeris time, orbit, and attitude.
       Earth Acquisition, the lowest level of safing
       responding to the most critical faults (e.g., battery
       at low state of charge) and no knowledge of ephemeris
       time, orbit, or attitude (with respect to the inertial
       reference frame) is assumed. The spacecraft is put
       into a slow rotation (one revolution every 3.5 hours)
       allowing the antenna suite to sweep past the Earth
       periodically regardless of location.
 
     Guidance and Control
     --------------------
       The primary functions of the guidance and control
       subsystem are to maintain spacecraft attitude and to
       execute propulsive maneuvers for spacecraft trajectory
       control. It consists of the spacecraft's attitude
       sensors including star cameras and Sun sensors
       integrated with controllers including reaction wheels.
       The system enforces two attitude safety constraints:
       the Sun Keep-In constraint that keeps the sunshade
       pointed towards the Sun to protect the spacecraft bus
       from extreme heat and the hot-pole keep-out constraint
       that protects components on the top deck from re-
       radiation of sunlight from the surface of Mercury.
 
       The sensor suite consists of star trackers, an IMU,
       and Sun sensors. The primary actuators for maintaining
       attitude control are four reaction wheels, each of
       which provides a maximum torque of 0.075 Nm and can
       store up to 7.5 Nms of momentum. Thrusters in the
       propulsion system are used for attitude control during
       TCMs and momentum dumps and may also be used as a
       backup system for attitude control in the event of
       multiple wheel failures.
 
       The G&C system also interfaces with actuators for
       three other spacecraft components to position them
       properly based on knowledge of the Sun, Earth, and
       target planet directions relative to the spacecraft.
       These are the two solar array drive assemblies; the
       phased array antenna; and the pivot platform for the
       Mercury Dual Imaging System (MDIS) instrument. In
       addition, an interface to the Mercury Laser Altimeter
       (MLA) instrument provides a range and 'slant angle'
       used to set the instrument's internal configuration
       parameters for surface observations.
 
     Radio Frequency (RF) Telecommunications
     ---------------------------------------
       The RF telecommunications subsystem consists of
       redundant General Dynamics small deep space
       transponders, solid-state power amplifiers, phased-
       array antennas, and medium- and low-gain antennas.
       The phased-array antennas have no mechanical
       components that could fail in the extreme thermal
       environment of Mercury. They are designed to work at
       the 350 degrees C temperatures to be encountered.  The
       spacecraft is the first to utilize turbo coding for
       downlink, resulting in an extra 0.9 dB margin,
       corresponding to nearly a 25% increased in data
       return.
 
     Payload
     -------
       The MESSENGER payload consists of seven instruments:
       the Mercury Dual Imaging System (MDIS), the Gamma-Ray
       and Neutron Spectrometer (GRNS), the X-Ray
       Spectrometer (XRS), the Magnetometer (MAG), the
       Mercury Laser Altimeter (MLA), the Mercury Atmospheric
       and Surface Composition Spectrometer (MASCS), and the
       Energetic Particle and Plasma Spectrometer (EPPS).
       They are described in the MESSENGER MISSION.CAT file
       and in [SOLOMONETAL2007], as well as the individual
       instrument catalog files in the MESSENGER PDS
       archives.
 
       Instrument design was constrained along several
       dimensions.  The payload mass was limited 50 kg for
       the seven instruments. The demanding thermal
       requirements to stay warm enough during cruise and
       eclipse periods, but cold enough on orbit, were
       significant constraints. Although the spacecraft solar
       arrays generate ample power during the orbital phase
       of the mission, power is much lower during the early
       cruise phase, restricting the size of instrument
       heaters that could be used. Power is also limited to
       the battery during eclipse.
 
       The over-all spacecraft architecture specified
       distributed power and data processing for the
       instruments; each instrument had its own power supply
       and microprocessor. Redundant Data Processing Units
       (DPU)buffer all data interfaces between the payload
       elements and the spacecraft. Common, flight-ready
       power supply and processor boards, including basic
       software functions, are used by all but one
       instrument, allowing development of a common set of
       ground support equipment hardware and software. This
       system architecture allowed payload development and
       testing to proceed separately from the rest of the
       spacecraft.
 
 
   Instrument Host Overview - DSN
   ==============================
     The Deep Space Network is a telecommunications
     facility managed by the Jet Propulsion Laboratory of
     the California Institute of Technology for the U.S.
     National Aeronautics and Space Administration (NASA).
 
     The primary function of the DSN is to provide two-way
     communications between the Earth and spacecraft
     exploring the solar system.  To carry out this
     function it is equipped with high-power transmitters,
     low-noise amplifiers and receivers, and appropriate
     monitoring and control systems.
 
     The DSN consists of three complexes situated at
     approximately equally spaced longitudinal intervals
     around the globe at Goldstone (near Barstow,
     California), Robledo (near Madrid, Spain), and
     Tidbinbilla (near Canberra, Australia).  Two of the
     complexes are located in the northern hemisphere while
     the third is in the southern hemisphere.
 
     Each complex includes several antennas, defined by
     their diameters, construction, or operational
     characteristics: 70-m diameter, standard 34-m
     diameter, high-efficiency 34-m diameter (HEF), and 34
     m beam waveguide (BWG).
 
     For more information see [ASMAR&RENZETTI1993].
 
   Instrument Host Overview - Spacecraft Clock Reset and Use of Clock
   Partitions
   ==================================================================
     A planned reset of the on-board clock of the MESSENGER spacecraft
     occurred on January 8, 2013. This was commanded by Mission Operations and
     was done because the integer seconds part of the on-board mission-
     elapsed-time (MET) counter is not long enough to contain the larger MET
     values that would occur due to the extended mission. The MESSENGER team
     elected to command the clock reset and set MET to a small non-zero value
     to prevent disruptions in on-board timekeeping and other effects (that
     might have occurred if the clock were allowed to automatically rollover
     to 0 in early 2013) and to ensure that the MET counter would accomodate
     the remaining extended mission.
 
     As a result of the spacecraft clock reset, a discontinuity was introduced
     and MET values are no longer guaranteed to be unique throughout the
     mission. This ambiguity is resolved in ground processing by the use of
     SPICE 'clock partitions' (partition 1 for pre-reset METs and partition 2
     for post-reset METs) in the Spacecraft Clock (SCLK) kernel (which
     supports mapping MET to other time forms using SPICE routines as
     described below) and with MET values stored in PDS products, labels, and
     for some instruments, product file names.  For MET values in products or
     labels,  a '1/' or '2/' preceding MET indicates the partition, as in:
 
     SPACECRAFT_CLOCK_START_COUNT   = '1/265485874'
     SPACECRAFT_CLOCK_STOP_COUNT    = '2/100005'
 
     When using SPICE routines, clock partition numbers should be included
     with MET input values. METs expressed without an explicit partition
     number are associated with clock partition 1 by default. Use of clock
     partition numbers in file names for some MDIS products is described in
     the MDIS EDR and CDR/RDR SIS documents with those data sets.
 
     Spacecraft Clock (SCLK) SPICE Kernel
     -------------------------------------
     The SCLK SPICE Kernel provides information that correlates mission
     elapsed time (MET) as measured by the spacecraft's on-board clock with
     Terrestrial Dynamical Time (TDT) as defined by the International
     Astronomical Union (IAU). (TDT was later redefined by the IAU and
     renamed 'Terrestrial Time' with the acronym 'TT.' However, that acronym
     is ambiguous in the SPICE context.). A 'partition' is a segment of time
     when the MET count increments continuously. A single clock partition can
     continue for years. When a discontinuity in MET occurs, a new partition
     is defined. MET discontinuities can occur for a number of reasons and can
     result in either a jump forward in MET or a jump backwards.
     Spacecraft clock jumps or discontinuities can be either the result of
     anomalies or they can be deliberately commanded. When such a
     discontinuity occurs, the previous correlation of MET to TDT is not valid
     from that point forward. A new clock partition must be created in order
     to correctly associate MET with TDT. The SCLK contains a list of all
     partitions that have been defined and specifies the MET values at which
     each ends. SPICE takes the partitions into account when computing the
     encoded SCLK representations of MET that make up the first field in each
     SCLK record 'triplet.' Because of this, the encoded SCLK values in the
     kernel increment steadily regardless of partition changes.
 
     Prior to the MESSENGER spacecraft clock reset, the MESSENGER SCLK kernel
     defined a single partition (partition 1). A second post-reset partition
     was introduced (partition 2) shortly before the reset. SCLK kernels from
     that time forward include both partitions.
 
     The MET partition change is largely transparent to users of SPICE and the
     SCLK kernel (with the exception of users who are converting raw MET
     counts), since the MET values in the kernel are provided in encoded SCLK
     form.

        