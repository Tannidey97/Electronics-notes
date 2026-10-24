# Bipolar Junction Transistor(BJT)
A bipolar junction transistor (BJT) is made of three doped semiconductor regions, the emitter, base, and collector, separated by two PN junctions. It comes in two types: NPN, with a p region between two n regions, and PNP, with an n region between two p regions. The emitter is heavily doped, the collector is moderately doped, and the base is lightly doped and very thin. This design is what makes the transistor work.

## BJT Transistor figure 
https://github.com/Tannidey97/Electronics-notes/blob/main/Transistor%20diagram.jpg

# Operation 

First, the emitter is heavily doped n-type, so it has a huge number of free electrons. Because the BE junction is forward biased, these electrons easily move across it into the base.
Second, the base is p-type, thin, and lightly doped, so it has very few holes. A small percentage of the incoming electrons recombine with those holes. The recombined electrons leave the base through the base lead, and this forms the small base current (I_B).
Third, most electrons do not recombine, because the base is so thin and has so few holes. They reach the reverse-biased BC junction, where the positive collector supply voltage attracts them and sweeps them across into the collector. This forms the large collector current (I_C).
Finally, the electrons travel through the external circuit and return to the emitter, along with the base current, completing the loop.

## Currents

https://github.com/Tannidey97/Electronics-notes/blob/main/Schematic%20symbol.jpg

The emitter current is what's injected into the base, and it splits into a small part (I_B) and a large part (I_C). So I_E = I_C + I_B, and I_E is only slightly larger than I_C.

$$I_E = I_C + I_B$$

# Cut off

A transistor is in cutoff when the base current is zero ($$I_B$$ = 0). This happens when the base-emitter (BE) junction is not forward biased enough to conduct, meaning $$V_{BE}$$ is below about 0.7 V for silicon. 
Under this condition, only a very small collector leakage current, $$I_{CEO}$$, flows. It is caused mainly by thermally produced carriers. The subscript CEO means collector-to-emitter with the base open. Because $$I_{CEO}$$ is extremely small, it is usually neglected in circuit analysis. So $$I_C$$ ≈ 0, and the whole supply voltage appears across the transistor:

**$$V_{CE}$$ ≈ $$V_{CC}$$**

In cutoff, the BE junction is not forward biased (it is either unbiased or reverse biased), and the base-collector (BC) junction is reverse biased.The transistor behaves like an open switch (OFF).





