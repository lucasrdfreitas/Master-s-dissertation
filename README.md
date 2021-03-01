# Gapless excitations in Kitaev materials with defects

This is a repo for my master's dissertation.



## Abstract

A quantum spin liquid is a magnetic phase of matter that is remarkable for its ground state long-range entanglement and fractional excitations. 
A  quantum spin liquid  appears in the well-known Kitaev honeycomb spin-half model. 
In a magnetic field, there is a phase transition to a topological phase with an energy gap in the bulk and chiral Majorana fermions at the edge. 
However, recent \acrlong{nmr} experiments suggest excitations without a gap in this phase, signalled by the cubic temperature dependence of the spin-lattice relaxation 
rate at low temperatures. 

In this work, I propose a mechanism to account for this experimental result. 
I use the localization of chiral Majorana modes in defects to explain the presence of gapless modes in the bulk. 
Treating the weak interaction between the chiral modes in the defects within a mean-field approximation, 
I find that these modes remain gapless when the interaction is below a critical value that depends on the magnetic field strength. 
I used the effective low-energy theory to calculate the spin-lattice relaxation rate and found a behavior that agrees with the experimental result.

**Keywords:** Kitaev model, Quantum spin liquids, Majorana fermions, Mean-field, Nuclear relaxation rate.

<br>
<hr>
<br>

## Introduction

The  interplay  of  topology  and  strongly  correlated  phenomena  gives  rise  to  fascinating physics such as the fractionalization of elementary particles.  An important example  is  the  fractional  quantum  Hall  effect,  in  which  the  electronic  degrees  offreedom split into quasiparticles with fractional electron charge.  Another prominent example  is  the  central  theme  of  this  work:  the  quantum  spin  liquid  (QSL)  [2–5]. In  magnetic  insulators,  these  phases  of  matter  exhibit  long-range  coherence,  butfluctuation prevents the formation of magnetic order even at zero temperature.

A  remarkable  example  of  QSL  is  the  Kitaev  spin  liquid  (KSL)  proposed  asa  toy  model  by  A.  Kitaev  in  2006  [6].   This  strongly  interacting  spin  system  hasas its elementary excitation $$Z_2$$-vortices and Majorana fermions.  Upon applying amagnetic  field,  the  Majoranas  become  gapped  with  a  Chern  insulator  spectrum. The  non-trivial  topology  of  this  insulator  gives  rise  to  chiral  Majorana  modes  atthe edge.  Unlike the fractional quantum Hall effect, the edge modes with oppositechiralities in KSL are electrically neutral. 

In previous work, [7], Kitaev had proposed that non-Abelian anyons could beused to realize a physical error-correction quantum code.  The anyonic system pro-vides a realization of a quantum memory that is protected from decoherence.  Thisremarkable property raised attention for theoretical models with this type of par-ticle since the current major limitation to construct a useful quantum computer isthe frequent errors caused by decoherence.  The quantum computers (theoretically) made using these models are named topological quantum computers [8, 9].  The Ki-taev  model  was  constructed  with  the  purpose  of  creating  a  two-dimensional spin model whose elementary were non-Abelian anyons.

The Kitaev model was not created with a physical realization in mind.  Nev-ertheless, a few years later Jackeli and Khaliullin [10] proposed a mechanism for aMott insulator with dominant Kitaev interaction.  The first studied materials werethe iridates,  $$A_2IrO_3$$ (A = Na,Li),  which realize the Kitaev model plus additionalsmall non-Kitaev interaction.  The model that include those non-Kitaev interactionsis called extended  Kitaev  model or J-K-Γ, J for the Heisenberg interaction,Kforthe Kitaev interaction, and Γ for the off-diagonal interactions.

Even though the non-Kitaev interactions are small in the iridate materials, they are  sufficient  to  drive  a  zigzag  order  for  weak  magnetic  fields  [11, 12].   Therefore, the  iridates  do  not  have  a  QSL  ground  state.   Furthermore,  for  strong  fields,  thematerial goes through a phase transition to a paramagnetic phase, a trivial partially polarized state.  There is a small window of magnetic fields in which a QSL mayexist.  A similar situation happens for ruthenium trichloride (α-RuCl3).  However, it is slightly better since the Néel temperature (T_N) is much smaller for this ruthenium material than for iridate ones.

One experimental group tested the spin-orbit Mott insulator α-RuCl_3 and found evidence for a thermal quantum Hall effect [1, 13].  While the elementary excitation of KSL are neutral, they can carry energy and therefore contribute to heat transport. The experiment was done using a temperature gradient. The theory for KSL predicts that the α-RuCl_3 exhibits a quantization of the transverse thermal conductivity $$κ_{xy}$$. The experimental results are not sharp and clear, but the authors of [13] believe they found the thermal Hall effect in a region of moderate magnetic fields 7–9T. The value measured for $$κ_{xy}$$ is not equal to the ideal conductivity of an isolated edge mode.There are proposals to explain this difference because of the coupling between thephonons and the Majorana edge modes [14, 15]. 

A recent nuclear magnetic resonance (NMR) experiment found unexpected results [16].  From the theory of Kitaev materials,α-RuCl_3 should behave as a gappedQSL under not too strong magnetic fields.  This behavior was experimentally verified in thermal Hall measurements in [1, 13] and specific heat measurements [17]. However,  this NMR experiment found a spin-lattice relaxation rate of $$1/T_1 ∝ T^3$$, which is rather expected for a gapless fermionic system.  In the words of the authorsof [16]:  <q> *our  NMR  results  show  unequivocally  that  the  spin  excitations  themselvesare  gapless,  and  thus  such  proximate  Kitaev  physics  appears  to  be  excluded. [...]  This result cannot be reconciled with the behavior of conventional quantum magnetsor of the pure or generic Kitaev QSL* </q>.

Another NMR experiment [18] claimed to observe a behavior $$1/T_1 ∝ Exp(−∆/T)$$, but only in the regime of large magnetic fields where the gap must be associated with magnons in the trivial paramagnetic phase.  In [19], the temperature dependence of $$1/T_1$$ was fitted to a double exponential in an attempt to extract two different energy scales associated with Majorana fermions and vortices.  A very recent thermal trans-port experiment, [20], founded evidence for defect-induced low-energy excitations in the longitudinal heat conductivity for α-RuCl3.

On theoretical grounds, Kitaev materials under moderate magnetic fields shouldexhibit  gapless  Majorana  fermions  at  the  edge,  but  the  NMR  experiments  on  anideal  material  would  probe  the  bulk  excitation  which  is  gapped.   In  this  work,  I explore the possibility that the observed gapless mode in the bulk is due to Majorana fermions localized along with linear defects in the material. It is known that stackingfaults in layered materials may induce the formation of linear defects such as partial dislocations [21].  Indeed, α-RuCl3 is a quasi-two-dimensional material with weakly interacting layers that can easily slip on one another producing stacking faults [22–25].

This  work  is  a  study  of  linear  defects  in  the  pure  Kitaev  model.   As  a  first theoretical model, I focus on a particular type of linear defects in which the structureresembles a zigzag edge.  The toy model for this defect consists of seaming two semi-infinite  KSL.  At  my  starting  point,  both  subsystems  contain  chiral  edge  modes,which I then couple by an exchange interaction that is weaker along with the defectthan  in  the  bulk.   My  model  is  inspired  by  Ref.  [26],  which  noted  that  there  is a  critical  value  of  the  exchange  interaction  between  edges  below  which  the  chiral modes remain decoupled.  From the point of view of the low-energy effective theory, the  reason  is  that  the  weak  interaction  between  emergent  Majorana  fermions  is irrelevant in the renormalization group sense.

In  contrast  to  the  field  theoretical  arguments  of  Ref.  [26],  here  I  first  study the critical condition for seaming the one-dimensional Majorana modes directly in the  lattice  model.   First,  I  calculate  the  spectrum  using  a  self-consistent  mean-field  approximation  for  the  exchange  interaction  along  with  the  defect.   Having identified the regime of decoupled gapless modes, I proceed by explicitly deriving the representation of the spin operator in the low-energy sector as a Majorana fermion bilinear. Following, I then use the effective field theory to compute the dynamicalspin-spin correlation function which determines the spin-lattice relaxation rate atlow temperatures.  I find the power-law dependence $$1/T_1 ∝ T^3$$, in agreement with the experimental results of Ref. [16].

This dissertation is organized as follows.  In chapter 2, I will set the notationand review the important aspects of the Kitaev model.  Complementary, the descrip-tion of the model in a more convenient geometry with zigzag edges is presented in chapter 3.  The defects are described in chapter 4 in which mean-field approximationis used to deal with the interaction across the <q>edges</q> of the defect.  The approximation gives ground to describe the low-energetic excitation localized in the defect asMajorana fermions, the passage from the microscopic theory to this effective theory is  described  in  chapter  5.   The  spin-lattice  relaxation  rate,  $$1/T_1$$,  is  calculated  in chapter 6.






