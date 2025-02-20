
 
    Instrument Host Overview
    ========================
 
      The Pioneer Venus mission objectives dictated the requirement
      for two spacecraft designs designated the Orbiter and the
      Multiprobe.  (The Multiprobe is defined as the Bus with the one
      Large Probe and three identical Small Probes attached in the
      launch/cruise configuration.) The conceptual designs of these
      spacecraft resulted from Phase B studies conducted from October
      1972 to July 1973, and after selection of the spacecraft
      contractor, Hughes Aircraft Company, in February 1974, a
      spacecraft conceptual design review was conducted in November
      1974.
 
      The Orbiter and Multiprobe utilized the same designs to the
      maximum extent possible to minimize costs.  In addition,
      designs of subsystems or portions of subsystems from previous
      spacecraft designs (such as OSO and Intelsat) were utilized to
      the maximum extent possible with little or no modifications.
      This commonality in the two spacecraft designs also resulted in
      certain amounts of commonality in ground test equipment and
      test software as well as commonality in spacecraft flight
      operations and associated software.
 
      Extracted from:
 
      NOTHWANG, George J.,'Pioneer Venus Spacecraft Design and
      Operation', IEEE Transactions on Geoscience and Remote Sensing,
      vol.  GE-18, No.  1, January 1980
 
 
    Platform Descriptions
    =====================
 
      Also from [NOTHWANG1980]:
 
      ORBITER
      -------
 
      The Orbiter spacecraft consists of the following subsystems and
      functions: Mechanical Function (including the Spacecraft Structure),
      Thermal Function (accomplished by the Structure/Harness Subsystem),
      Controls Subsystem, Propulsion Subystem, Data Handling Subsystem,
      Command Subsystem, Communications Subsystem, and Power Subsystem.
 
        Mechanical
        ----------
 
        The mechanical features of the spacecraft can be described by six
        basic assemblies. The despun antenna assembly, the bearing and
        power transfer assembly (BAPTA), the BAPTA support structure,
        equipment shelf, substrate (solar array), orbit insertion motor
        (OIM) and its case, and thrust tube. The shape and equipment layout
        conform to the basic mechanical requirements of a spin-stabilized
        vehicle. The solar cells on the cylindrical solar panel, antenna
        orientations, and thrust vector orientations provide efficient
        power, communications, and maneuverability while the Orbiter is
        spinning in its cruise and orbit attitudes.
 
        Thermal
        -------
 
        The thermal design is based on isolating the equipment from the
        external solar extremes experienced during the mission. (Solar
        intensity increases by a factor of 1.98 from Earth to Venus.)
        Commandable heaters are provided to maintain the orbit insertion
        motor and safe and arm device within their specified temperature
        ranges, to prevent possible freezing of hydrazine monopropellant,
        and to make up heat balance should there occur an inadvertent trip
        of nonessential spacecraft loads. Fifteen thermostatically
        controlled thermal louvers are mounted on the aft side of the
        equipment shelf beneath units having high dissipations.
 
        Controls
        --------
 
        The controls subsystem provides the sensing logic and actuators
        to accomplish the following stabilization, control, and reference
        functions:
	  a) spin axis attitude determination (via use of slit
	     field-of-view type sun sensors and star sensors), science
	     roll reference signals generation, and spin period
	     measurement;
          b) control of thrusters for spin axis attitude maneuvers, spin
             speed control, and spacecraft velocity maneuvers;
          c) high-gain antenna azimuth despin control and elevation
             positioning to a desired earth line-of-sight pointing;
             additionally, antenna slew control for open-loop tracking of
             the Earth line-of-sight;
          d) magnetometer sensor deployment;
          e) nutational damping, via use of a partially filled tube of
             liquid Freon E3.
 
        Propulsion
        ----------
 
        The propulsion subsystem provides the hydrazine monopropellant
        storage, pressurization, distribution lines, isolation valves,
        filtering, and thruster assemblies used to accomplish Orbiter
        maneuvers throughout the mission.
 
        Data Handling
        ---- --------
 
        The data handling subsystem conditions and integrates into command-
        selectable (choice of thirteen fixed and one programmable) formats,
        all analog and digital telemetry data (248 assigned channels)
        originating in the subsystems and science instruments. The selected
        format of the all-digitized data modulates a 16384-Hz subcarrier
        at a command-selectable (choice of thirteen rates between 8 and
        4096 bps) bit rate. The resulting information is routed to the
        communications subsystem for modulation of the downlink S-band
        carrier. The data handling subsystem includes a data memory,
        consisting of two data storage units (DSU), that is intended
        primarily for use during any occultation. Data are stored or read
        out at the commanded bit rate. Each DSU has a capacity of 524,288
        bits (equivalent to 1024 telemetry minor frames).
 
        Command
        -------
 
        The command subsystem decodes all commands received via the
        communications subsystem at the fixed rate of 4 bps, and either
        stores the command for later execution or routes the command in
        real time to the addressed destination. Each of the 381 assigned
        commands is either completely decoded (discrete-type command) by
        the command subsystem and the execution command generated, or is
        partially decoded (quantitative-type command) by the command
        subsystem and the command is routed to the addressed destination
        for final decoding.
 
        Communications
        --------------
 
        The communications subsystem provides radiation reception and
        transmission capabilities for the command and telemetry
        information. The uplink command capability is maintained by
        modulating an S-band carrier of approximately 2.115 GHz. The
        downlink telemetry modulates an S-band carrier of approximately
        2.295 GHz. There are two redundant reception channels; each
        includes a hemispherically omnidirectional antenna (aft or forward)
        that spatially supplements the other to produce total spatial
        coverage. Optionally by command, the forward antenna is replaceable
        by a high-gain antenna or a high-gain back-up antenna.
 
        The S-band downlink is assignable by command to any one of the aft
        or forward omnidirectional antennas, or to the high-gain or high-
        gain back-up (directional) antennas. Its frequency is a multiple of
        the uplink frequency; or in the absence of an uplink signal, it is
        a multiple of a crystal oscillator located in the receiver. The
        downlink may also be transmitted via any one of, or some pairs of,
        four 10-W power amplifiers.
 
        There is an additional transmitter in the X-band range (the
        frequency is 11/3 of the S-band downlink frequency) that is for
        use in occultation measurements. The transmission is unmodulated
        through the high-gain antenna only.
 
        Power
        -----
 
        The power subsystem provides semiregulated 28V +/- 10 percent to
        all spacecraft loads (including science instruments). The primary
        source of power is the main solar array. When the solar panel
        output cannot provide adequate power for all spacecraft loads (at
        low sun angles and during eclipses), the two nickel/cadmium
        batteries (each rated at 7.5 Ah full capacity) come on line
        automatically through the discharge regulators. Battery energy is
        replenished through a small boost charge array. The power interface
        unit provides power switching for the propulsion heaters and OIM
        heaters. It also contains fuses for these circuits and the science
        instruments input power lines.
 
        Power is distributed on four separate power buses. If a spacecraft
        overcurrent condition or under-voltage on either battery occurs,
        loads are removed to protect the spacecraft from potential
        catastrophic failure by tripping off buses in the following
        sequence: science, switched loads, and transmitter. This leaves
        only those loads that are absolutely essential to spacecraft
        survival in a continuously powered ON mode. The RF transmitters and
        exciters are on the transmitter bus. Controls and data handling
        units are on the switched loads bus. Scientific instruments are on
        the science bus. Command units, OIM and propulsion heaters, power
        conditioning units, and spacecraft receivers are on the essential
        bus. Excitation for the pyro bus is derived from a battery tap
        located 16 cells (of a total of 24) from the ground reference
        level. The bus voltage is limited to 30.0 V by seven shunt limiters
        that dissipate all excess solar panel capacity in load resistors
        mounted on the solar panel substrate and equipment shelves.

        