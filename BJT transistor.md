# Bipolar Junction Transistor(BJT)
A bipolar junction transistor (BJT) is made of three doped semiconductor regions, the emitter, base, and collector, separated by two PN junctions. It comes in two types: NPN, with a p region between two n regions, and PNP, with an n region between two p regions. The emitter is heavily doped, the collector is moderately doped, and the base is lightly doped and very thin. This design is what makes the transistor work.

## BJT Transistor figure 
https://github.com/Tannidey97/Electronics-notes/blob/main/Transistor%20diagram.jpg

# Operation 

### NPN Transistor 

First, the emitter is heavily doped n-type, so it has a huge number of free electrons. As the BE junction is forward biased, these electrons can easily move across it into the base.
Second, the base is p-type, thin, and lightly doped, so it has very few holes. A small percentage of the incoming electrons recombine with those holes. To keep this going, the base lead removes electrons from the base, creating new holes. This forms the small base current ($I_B$).
Third, most of the electrons do not recombine, because the base is so thin and has so few holes. They reach the reverse-biased BC junction, where the positive collector supply voltage attracts them and sweeps them across into the collector. This forms the large collector current ($I_C$).
Finally, the electrons travel through the external circuit and return to the emitter, along with the base current, completing the loop.

### PNP Transistor 

In a PNP transistor, the emitter is heavily doped p-type, so it contains a large number of holes. The emitter is at a higher voltage than the base, making the BE junction forward biased. As a result, holes move from the emitter into the base.
The base is thin and lightly doped n-type, so it contains very few electrons. Only a few holes recombine with electrons in the base, producing a small base current ($I_B$).
Most of the holes cross the thin base without recombining. When they reach the reverse-biased BC junction, they are attracted into the collector, producing a large collector current ($I_C$).
Finally, the external circuit completes the current flow by supplying electrons to replace the holes. Thus, a large collector current and a small base current flow in the PNP transistor.

## Currents

https://github.com/Tannidey97/Electronics-notes/blob/main/Schematic%20symbol.jpg

## Currents

**In an NPN transistor, the electrons from the emitter divide into a small part that leaves through the base and a large part that goes to the collector. In terms of conventional current, $I_B$ and $I_C$ flow into the transistor and add up to $I_E$, which flows out of the emitter.**  

**And in a PNP transistor, the holes from the emitter divide into a small part that recombines in the base and a large part that goes to the collector. In terms of conventional current, $I_E$ flows into the transistor and splits into $I_B$ and $I_C$, which flow out of it.**  

Both type of transistors follows the sane current formula :  

***$I_E$ = $I_C$ + $I_B$***

# Cutoff

A transistor is in cutoff when the base current is zero ($$I_B$$ = 0). This happens when the base-emitter (BE) junction is not forward biased enough to conduct, meaning $$V_{BE}$$ is below about 0.7 V for silicon. 
Under this condition, only a very small collector leakage current, $$I_{CEO}$$, flows. It is caused mainly by thermally produced carriers. The subscript CEO means collector-to-emitter with the base open. Because $$I_{CEO}$$ is extremely small, it is usually neglected in circuit analysis. So $$I_C$$ ≈ 0, and the whole supply voltage appears across the transistor:

**$$V_{CE}$$≈$$V_{CC}$$**

In cutoff, the BE junction is not forward biased (it is either unbiased or reverse biased), and the base-collector (BC) junction is reverse biased.The transistor behaves like an open switch (OFF).

# Saturation 

If $$V_{CC}$$ and $$R_C$$ are fixed and never change. Only the base supply $$V_{BB}$$ is increased. When $$V_{BB}$$ increases, the base-emitter junction is pushed harder in the forward direction, so the base current I_B increases. As $$I_B$$ increases, the heavily doped emitter supplies more current carriers (free electrons) into the base.

The base is thin, so most of these electrons pass through to the collector. This is why the collector current depends on the base current: $$I_C$$ = $$β_{DC}$$ × $$I_B$$. When I_B increases, $$I_C$$ also increases.

The collector current flows through $$R_C$$ and produces a voltage drop across it ($$I_C$$ × $$R_C$$). Since $$V_{CC}$$ is fixed, a larger drop across $$R_C$$ leaves less voltage across the transistor, so $$V_{CE}$$ decreases. This is given by $$V_{CE}$$ = $$V_{CC}$$ − $$I_C$$ × $$R_C$$.

$$V_{CE}$$ keeps falling until it reaches its saturation value, $$V_{CE}$$(sat), which is only a few tenths of a volt. At this point the base-collector junction becomes forward biased. Now $$I_C$$ cannot increase any further, even if $$I_B$$ keeps increasing, because $$I_C$$ is limited by $$V_{CC}$$ and $$R_C$$ and not by $$I_B$$. Because of this, the relation $$I_C$$ = $$β_{DC}$$ × $$I_B$$ is no longer valid in saturation.

In saturation, both the base-emitter and base-collector junctions are forward biased, V_CE is almost zero, and I_C is at its maximum. The transistor acts like a closed switch (ON).
